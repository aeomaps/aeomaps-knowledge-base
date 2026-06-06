---
title: "Aterramento Elétrico: Guia Completo de Projeto, Normas e Proteção"
slug: aterramento-eletrico-guia-completo
date: 2026-06-06 07:00:00
categories: Aterramento
tags: aterramento, BEP, condutor PE, eletrodo, equipotencialização, IT, NBR 5410, NBR 5419, proteção, SPDA, TN, TT
source: aeomaps.com.br/aterramento-eletrico-guia-completo/
---

### Definição técnica de aterramento

Aterramento elétrico é a ligação intencional de um ponto do sistema elétrico ao solo, estabelecendo uma referência de potencial e um caminho para escoamento de correntes de falta e descargas atmosféricas. O aterramento não é um acessório — é parte estrutural da proteção de pessoas e equipamentos.

Um sistema de aterramento compreende: eletrodo(s) de aterramento, condutores de aterramento, condutores de proteção (PE), barramento de equipotencialização principal (BEP) e as ligações equipotenciais suplementares.

### Seis funções do aterramento

O aterramento cumpre funções simultâneas e complementares em uma instalação elétrica:

**1. Referência de potencial:** estabelece o zero volt do sistema, permitindo que tensões fase-terra e neutro-terra sejam definidas e medidas.

**2. Proteção contra contatos indiretos:** ao conectar as massas metálicas (carcaças, gabinetes) ao PE, garante que uma falta de isolamento provoque corrente suficiente para atuar o dispositivo de proteção (DR, disjuntor).

**3. Escoamento de descargas atmosféricas:** o subsistema de aterramento do SPDA drena a corrente do raio para o solo, limitando sobretensões na estrutura.

**4. Escoamento de surtos e correntes transitórias:** protege equipamentos contra sobretensões de manobra e surtos induzidos, em conjunto com DPS (Dispositivos de Proteção contra Surtos).

**5. Proteção contra tensões transferidas:** limita tensões de passo e toque que surgem durante faltas à terra ou descargas atmosféricas.

**6. Estabilização de potencial em sistemas de potência:** em subestações e sistemas de geração, o aterramento do neutro define o comportamento do sistema durante faltas (corrente de curto, seletividade).

### Conceitos fundamentais

**[Tensão de contato](/tensao-passo-toque-protecao-pessoas):** diferença de potencial entre uma massa acessível e o ponto do solo onde a pessoa está. A NBR 5410 define limites: 50 V em condições normais, 25 V em condições especiais (locais úmidos, canteiros).

**Tensão de passo:** diferença de potencial entre dois pontos do solo separados por 1 metro na direção radial ao eletrodo. Durante descargas atmosféricas, pode atingir valores letais nas proximidades da haste. Detalhes em [tensão de passo e toque](/tensao-passo-toque-protecao-pessoas).

**Equipotencialização:** conexão de todas as massas, elementos condutores estranhos à instalação (tubulações, ferragens, estruturas metálicas) e eletrodos de aterramento a um ponto comum (BEP), minimizando diferenças de potencial acessíveis.

**Efeitos fisiológicos da corrente:**

CorrenteEfeito~1 mAPercepção~5 mAEletrização10 mATetanização25 mAParada respiratória60–75 mAFibrilação ventricular
### Esquemas de aterramento: TT, TN e IT

A primeira letra indica o aterramento da fonte (T = aterrado, I = isolado). A segunda indica o aterramento das massas (T = aterrado independentemente, N = ligado ao neutro).

**TT — Terra-Terra:**

O neutro da fonte é aterrado. As massas do consumidor são aterradas por eletrodo independente. A corrente de falta retorna pelo solo. O DR é obrigatório para proteção contra contatos indiretos.

**TN-S — Terra-Neutro Separado:**

Neutro aterrado na origem. Condutor PE separado do neutro (N) em toda a instalação. Proteção por sobrecorrente (disjuntores/fusíveis) é viável, mas DR é recomendado.

**TN-C — Terra-Neutro Combinado:**

Neutro e PE combinados em um único condutor PEN. Seção mínima: 10 mm² Cu ou 16 mm² Al. Proibido em circuitos com seção inferior. Proibido em locais com risco de explosão.

**TN-C-S — Configuração brasileira típica:**

PEN a montante (entrada), separação em PE e N a partir de um ponto (geralmente o BEP do quadro geral). Configuração predominante em instalações residenciais e comerciais no Brasil.

**IT — Isolado:**

Neutro isolado da terra (ou aterrado por alta impedância). O primeiro defeito não provoca corrente perigosa. Exige monitoramento contínuo de isolamento. Aplicação típica: salas cirúrgicas, processos industriais onde a continuidade é crítica.

### Eletrodos de aterramento

**Eletrodos naturais (preferenciais):**

A NBR 5410 e a NBR 5419 incentivam o uso de elementos já existentes na construção como eletrodos de aterramento:

- Ferragem de fundação: a armadura do concreto em contato com o solo constitui um eletrodo de baixa resistência. A resistência da ferragem de fundação pode ser da ordem de 0,25 Ω em construções de grande porte.
- Tubulações metálicas de água em contato direto com o solo (não válido para tubulações plásticas ou com juntas isolantes).
- Estacas e blocos de concreto armado.

**Eletrodos fabricados:**

- [Hastes copperweld](/haste-aterramento-tipos-instalacao-medicao): padrão brasileiro, 5/8" ou 3/4" × 2,40 ou 3,00 m. Complementares ao anel na NBR 5419:2026.
- Cabo de cobre nu enterrado: mínimo 50 mm² (NBR 5419:2026). Enterrado a 50 cm de profundidade.
- Fitas ou chapas de cobre.
- Anel de aterramento: obrigatório pela NBR 5419:2026, enterrado no perímetro da edificação.

**Mudanças da NBR 5419:2026:**

- Anel de aterramento obrigatório (não mais aterramento pontual com hastes isoladas)
- Proibição de aço zincado na transição concreto-solo (corrosão galvânica)
- Cabo de cobre mínimo: 50 mm²
- Sem prescrição de valor máximo fixo de resistência de aterramento

### Barramento de Equipotencialização Principal (BEP)

O BEP é a barra central do sistema de equipotencialização. Localizado na entrada da instalação, recebe as conexões de:

- Condutor de aterramento principal (ligação ao eletrodo)
- Condutores de proteção (PE) de todos os circuitos
- Condutor neutro (no ponto de separação PEN → PE + N, no esquema TN-C-S)
- Tubulações metálicas (água, gás, esgoto)
- Blindagens de cabos de telecomunicação
- DPS (Dispositivos de Proteção contra Surtos)
- SPDA (condutor de descida do para-raios)
- Armaduras de concreto acessíveis
- Estruturas metálicas da edificação

Dimensionamento mínimo do BEP: barra de cobre nu, ≥ 50 × 3 × 500 mm (largura × espessura × comprimento). Cabo de ligação ao eletrodo: ≥ 16 mm² Cu.

A nomenclatura correta é BEP (Barramento de Equipotencialização Principal). A sigla TAP (Terminal de Aterramento Principal) era usada antes da revisão de 2004 da NBR 5410.

### Dimensionamento do condutor de proteção (PE)

A seção do condutor PE é definida pela NBR 5410, Tabela 53:

Seção da fase S (mm²)Seção mínima do PE (mm²)S ≤ 16S (igual à fase)16 16S > 35S/2
Identificação: verde-amarelo (PE), azul com marcação verde-amarela nas extremidades (PEN).

A fórmula de cálculo por energia é: S = √(I²t) / K, onde I é a corrente de falta, t é o tempo de atuação da proteção e K é o fator do material do condutor.

### Valor de resistência de aterramento

Não existe [valor fixo universal de resistência de aterramento](/mito-10-ohms-resistencia-aterramento). A NBR 5410 calcula o valor admissível conforme o esquema:

- **TT:** RA × IΔn ≤ UL (onde IΔn é a sensibilidade do DR e UL é 50 V ou 25 V)
- **TN:** a medição de RA tem pouca relevância para proteção contra choques — o que importa é a impedância do laço de falta (Zs × Ia ≤ U₀)
- **IT:** critérios específicos conforme a condição de primeiro ou segundo defeito

A NBR 5419:2026 não prescreve valor máximo fixo para o SPDA. O dimensionamento prioriza geometria, material e continuidade do eletrodo.

### Medição e ensaios

**Resistividade do solo:** NBR 7117:2020, [método de Wenner](/resistividade-solo-metodo-wenner). Quatro hastes equidistantes, medição em 3+ direções, espaçamentos progressivos (1, 2, 4, 8, 16, 32 m). Fórmula: ρ = 2πaR.

**Resistência de aterramento:** NBR 15749, [método de queda de potencial com terrômetro](/haste-aterramento-tipos-instalacao-medicao). Eletrodo de potencial a 62% da distância ao eletrodo de corrente.

**Periodicidade de inspeção:**

Tipo de instalaçãoPeriodicidadeEdifícios e indústrias1 anoDemais estruturas3 anosCanteiro de obras (NR-18 grua)Semestral
### Normas técnicas aplicáveis

NormaTemaNBR 5410:2004Instalações elétricas de baixa tensãoNBR 5419:2026Proteção contra descargas atmosféricasNBR 7117:2020Medição de resistividade do soloNBR 15749:2009Medição de resistência de aterramentoNBR 17018:2023Instalações elétricas em canteiros de obrasNR-10Segurança em instalações e serviços em eletricidadeNR-18Condições de trabalho na construção
### Erros frequentes em projeto e execução

- Afirmar que "10 Ω" é o limite normativo universal — a NBR 5410 não prescreve esse valor
- Usar o neutro como PE (fio terra) — cria corrente nas carcaças
- Não conectar tubulações metálicas ao BEP — cria diferenças de potencial acessíveis
- Cravar hastes próximas demais (d 
Projeto de aterramento, adequação normativa ou diagnóstico de sistema existente? A equipe AEOMaps cobre desde a medição de resistividade até o dimensionamento completo.

**[Fale com um especialista pelo WhatsApp →](https://wa.me/5511925222281?text=Olá!%20Vim%20pelo%20guia%20completo%20de%20aterramento%20elétrico%20e%20preciso%20de%20orientação%20técnica.)**