---
title: "Sistemas TT, TN e IT: Diferenças, Normas e Quando Usar Cada Esquema de Aterramento"
slug: sistemas-tt-tn-it-diferencas
date: 2026-06-02 06:00:00
categories: Aterramento
tags: DR, esquema aterramento, IT, NBR 5410, neutro, PE, proteção, TN, TN-C-S, TT
source: aeomaps.com.br/sistemas-tt-tn-it-diferencas/
---

### O que define o esquema de aterramento

O esquema de aterramento descreve a relação entre o sistema de alimentação (transformador), o aterramento e as massas (carcaças metálicas) dos equipamentos. A NBR 5410:2004 adota a classificação internacional IEC, com duas letras:

**Primeira letra — situação da alimentação em relação à terra:**

- **T** (*Terre*): ponto da alimentação (neutro do transformador) diretamente aterrado
- **I** (*Isolé*): ponto da alimentação isolado da terra ou aterrado por impedância elevada

**Segunda letra — situação das massas em relação à terra:**

- **T**: massas aterradas diretamente, em eletrodo independente do aterramento da alimentação
- **N** (*Neutre*): massas conectadas ao ponto aterrado da alimentação (neutro) por meio do condutor de proteção

Essa combinação gera três famílias: TT, TN (com variantes TN-S, TN-C e TN-C-S) e IT. Cada uma exige dispositivos de proteção específicos e tem comportamento diferente na falta à terra.

### Sistema TT

No esquema TT, o neutro do transformador é aterrado pela concessionária e as massas da instalação consumidora são aterradas por um eletrodo independente.

**Características:**

- Dois aterramentos distintos: um na fonte (concessionária) e outro na instalação
- O caminho da corrente de falta inclui o solo — a impedância é alta
- A corrente de falta é tipicamente baixa (dezenas de ampères, não milhares)
- Disjuntores e fusíveis convencionais geralmente **não** conseguem detectar a falta à terra no tempo prescrito

**Proteção obrigatória:** o dispositivo DR (diferencial residual) é **obrigatório** em todos os circuitos do esquema TT. Sem DR, a falta à terra não é eliminada dentro do tempo de segurança.

**Critério de coordenação (NBR 5410):** a resistência de aterramento das massas (RA) deve satisfazer:

**RA × IΔn ≤ UL**

Onde:

- RA = resistência do eletrodo de aterramento das massas (Ω)
- IΔn = corrente diferencial residual nominal do DR (A)
- UL = tensão de contato limite (50 V em condições normais, 25 V em condições especiais)

**Tabela de RA máximo admissível (UL = 50 V):**

IΔn do DRRA máximo (Ω)30 mA1.667100 mA500300 mA167500 mA100
Esses valores mostram que no sistema TT, o aterramento não precisa ter resistência ultrabaixa — o DR é o protagonista da proteção. Um DR de 30 mA aceita aterramento de até 1.667 Ω. É por isso que [o mito dos 10 Ω](/mito-10-ohms-resistencia-aterramento) não se sustenta tecnicamente no esquema TT.

**Aplicação típica:** instalações residenciais alimentadas pela rede de distribuição da concessionária. É o esquema mais comum no Brasil para consumidores em baixa tensão.

### Sistema TN

No esquema TN, o neutro do transformador é aterrado e as massas são conectadas ao ponto aterrado da alimentação por meio do condutor de proteção (PE ou PEN). A corrente de falta retorna ao transformador pelo condutor metálico — não pelo solo.

**Características gerais:**

- A corrente de falta é alta (centenas a milhares de ampères) — é um curto-circuito fase-PE
- Disjuntores e fusíveis convencionais podem atuar como proteção contra falta à terra
- O DR é recomendado como proteção complementar, mas a norma não o exige em todos os circuitos

**Critério de coordenação (NBR 5410):** a impedância do laço de falta (Zs) deve garantir a atuação do dispositivo de proteção no tempo prescrito:

**Zs × Ia ≤ Uo**

Onde:

- Zs = impedância do laço fase-PE (Ω)
- Ia = corrente de atuação do dispositivo no tempo prescrito (A)
- Uo = tensão fase-neutro (V)

No esquema TN, **a medição de resistência de aterramento isolada não tem significado para a proteção contra choques** — o que importa é a impedância do laço fase-PE.

#### TN-S (Separado)

PE e neutro são condutores separados em toda a instalação. O PE é exclusivo para proteção e não conduz corrente de operação.

**Vantagens:** menor interferência eletromagnética (sem corrente de neutro no PE), melhor compatibilidade com equipamentos eletrônicos sensíveis, referência de terra mais limpa.

**Onde usar:** instalações com equipamentos eletrônicos, CPDs, automação industrial, telecomunicações, ambientes com exigência de [aterramento para eletrônicos](/aterramento-equipamentos-eletronicos-mtr).

#### TN-C (Combinado)

Um único condutor (PEN) acumula as funções de proteção e neutro. O PEN conduz corrente de desequilíbrio em operação normal.

**Restrições normativas:**

- Seção mínima do PEN: 10 mm² (cobre) ou 16 mm² (alumínio)
- O PEN nunca pode ser seccionado unilateralmente
- Não é permitido em condutores flexíveis
- Não é permitido em seções inferiores a 10 mm² Cu

#### TN-C-S (Combinado → Separado)

É a configuração padrão brasileira para instalações alimentadas em baixa tensão a partir de transformadores da concessionária.

**Funcionamento:** o condutor PEN chega da rede da concessionária até o quadro de entrada (medição). No quadro de entrada, o PEN é dividido em PE + N, que seguem separados por toda a instalação interna. A partir do ponto de separação, PE e N nunca são reconectados.

**Na prática:** o aterramento é feito no quadro de entrada, onde o [BEP](/bep-barramento-equipotencializacao) recebe a ligação do PEN, do eletrodo de aterramento, dos condutores PE dos circuitos e dos condutores de equipotencialização.

### Sistema IT

No esquema IT, a alimentação é isolada da terra (ou aterrada por impedância elevada >1.000 Ω). As massas são aterradas individualmente ou em grupos.

**Comportamento na primeira falta:** a corrente que circula é apenas a corrente de fuga capacitiva do sistema — tipicamente alguns miliampères. A instalação **não desliga** na primeira falta, mantendo a continuidade de serviço.

**Exigência normativa:** um dispositivo supervisor de isolamento (DSI) deve monitorar continuamente a resistência de isolamento e sinalizar (alarme visual e sonoro) a ocorrência da primeira falta.

**Aplicações:**

- Salas cirúrgicas e UTIs (NBR 13534) — continuidade de fornecimento é crítica
- Processos industriais contínuos (fornos, laminação)
- Minas e ambientes com atmosfera explosiva

### Comparativo consolidado

CritérioTTTN-STN-CTN-C-SITAterramento do neutroSimSimSimSimNão (isolado)Aterramento das massasIndependenteVia PEVia PENPEN→PE+NIndependenteCorrente de faltaBaixa (solo)Alta (condutor)Alta (condutor)Alta (condutor)Capacitiva (1ª falta)Proteção obrigatóriaDRDisjuntor/fusívelDisjuntor/fusívelDisjuntor/fusívelDSI + disjuntorUso típico BrasilResidencialIndustrial/CPDRede concessionáriaPadrão brasileiroHospitalar/industrial
### NBR 5419:2026 e o esquema de aterramento

**Anel de aterramento obrigatório:** a NBR 5419:2026 exige anel de aterramento ao redor da edificação — não mais aterramentos pontuais isolados. O anel deve ser enterrado a no mínimo 50 cm, em cabo de cobre nu de 50 mm² mínimo.

Essa exigência muda a prática anterior de aterrar o SPDA em hastes nos pontos de descida. O anel cria uma equipotencialização perimetral que beneficia todos os esquemas de aterramento (TT, TN e IT), reduzindo [tensões de passo e toque](/tensao-passo-toque-protecao-pessoas) durante descargas atmosféricas.

### Como escolher o esquema

**Residencial e comercial pequeno:** TN-C-S é o padrão quando alimentado pela rede da concessionária.

**Industrial com equipamentos eletrônicos sensíveis:** TN-S desde o transformador (dedicado).

**Hospitalar (salas cirúrgicas, UTI):** IT com transformador de isolamento e DSI. Obrigatório pela NBR 13534.

**Canteiro de obras:** TT com DR em todos os circuitos é a configuração mais segura para [instalações temporárias](/aterramento-canteiro-obras-nr10-nr18).

### Erros frequentes

**1. Confundir TN-C com "terra pelo neutro"**

No TN-C, o PEN é um condutor dimensionado e identificado. "Usar o neutro como terra" sem dimensionamento e sem identificação não é TN-C — é gambiarra.

**2. Não converter TN-C para TN-S no quadro de entrada**

Se o PEN chega da rede e continua como PEN nos circuitos internos com seção inferior a 10 mm², a instalação viola a NBR 5410.

**3. Instalar DR em circuito TN-C**

O DR mede a diferença entre fase e neutro+PE. No TN-C, o PEN carrega ambas as correntes — o DR pode disparar falsamente ou não atuar quando deveria.

**4. Assumir que TT é inferior ao TN**

O TT com DR é extremamente seguro — a corrente que o DR detecta (30 mA) é muito inferior à corrente de atuação de um disjuntor. O TT é o esquema preferido pela IEC para instalações residenciais em vários países.

### Conclusão técnica

O esquema de aterramento determina como a instalação responde a uma falta à terra e quais dispositivos de proteção são necessários. No Brasil, o TN-C-S é a configuração predominante. A escolha correta do esquema — e a proteção correspondente — é o fundamento de toda a [segurança elétrica da instalação](/aterramento-eletrico-guia-completo).

### Links relacionados

- [Diferença entre Terra, Neutro e Massa](/diferenca-terra-neutro-massa)
- [BEP](/bep-barramento-equipotencializacao)
- [O Mito dos 10 Ω](/mito-10-ohms-resistencia-aterramento)
- [Tensão de Passo e Toque](/tensao-passo-toque-protecao-pessoas)
- [Aterramento em Canteiro de Obras](/aterramento-canteiro-obras-nr10-nr18)
- [Aterramento para Eletrônicos](/aterramento-equipamentos-eletronicos-mtr)
- [Guia Completo](/aterramento-eletrico-guia-completo)

Precisa definir o esquema de aterramento (TT, TN ou IT) ou adequar uma instalação existente? A equipe AEOMaps analisa a configuração e orienta a escolha conforme a norma e o cenário real.

**[Fale com um especialista pelo WhatsApp →](https://wa.me/5511925222281?text=Olá!%20Vim%20pelo%20artigo%20sobre%20sistemas%20TT%20TN%20IT%20e%20preciso%20de%20orientação%20técnica.)**