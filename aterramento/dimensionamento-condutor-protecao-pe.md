---
title: "Como Dimensionar o Condutor de Proteção (Fio Terra): Tabela, Fórmula e Norma"
slug: dimensionamento-condutor-protecao-pe
date: 2026-06-05 11:00:00
categories: Aterramento
tags: condutor de proteção, cor, dimensionamento, equipotencialização, fio terra, NBR 5410, PE, PEN
source: aeomaps.com.br/dimensionamento-condutor-protecao-pe/
---

### O que é o condutor de proteção (PE)

O condutor de proteção — designado PE (do inglês *Protective Earth*) — é o condutor que conecta as massas dos equipamentos elétricos ao sistema de aterramento. Sua função é garantir que, em caso de falha de isolamento, a corrente de falta encontre um caminho de baixa impedância até o eletrodo de aterramento, permitindo a atuação dos dispositivos de proteção (disjuntor, DR, fusível).

O PE não conduz corrente em operação normal. Se houver corrente mensurável no PE durante operação regular, há defeito na instalação — e esse é um dos primeiros diagnósticos a fazer quando se detecta [diferença entre terra e neutro](/diferenca-terra-neutro-massa) comprometida.

A NBR 5410:2004 (seção 6.4.3) estabelece os critérios de dimensionamento do PE. Não se trata de escolha arbitrária: a bitola mínima é determinada pela seção do condutor fase do circuito ou, alternativamente, por cálculo térmico.

### Dimensionamento pela tabela simplificada (Tabela 53 da NBR 5410)

O método mais utilizado na prática é a tabela simplificada, aplicável quando PE e fase são do mesmo material condutor:

Seção do condutor fase S (mm²)Seção mínima do PE (mm²)S ≤ 16S (igual à fase)16 16S > 35S/2
**Exemplos de aplicação direta:**

CircuitoFase (mm²)PE mínimo (mm²)Iluminação residencial1,51,5Tomadas gerais2,52,5Chuveiro elétrico (5.500 W)4,04,0Ar-condicionado 12.000 BTU2,52,5Alimentador de quadro 40 A1010Alimentador de quadro 63 A1616Alimentador industrial 100 A2516Alimentador industrial 200 A7035Alimentador subestação 500 A18595
Quando o PE não é do mesmo material que o condutor fase (por exemplo, fase em cobre e PE em alumínio), a seção deve ser corrigida para garantir condutância equivalente. O alumínio tem condutividade aproximadamente 60% da do cobre — um PE de alumínio equivalente a 16 mm² de cobre precisa ter no mínimo 25 mm².

### Dimensionamento por cálculo térmico (fórmula adiabática)

Para situações onde a tabela simplificada não se aplica ou quando se deseja otimização, a NBR 5410 permite o cálculo pela fórmula adiabática:

**S = √(I² × t) / K**

Onde:

- **S** = seção mínima do PE (mm²)
- **I** = corrente de falta presumida (A) — corrente de curto-circuito no ponto
- **t** = tempo de atuação do dispositivo de proteção (s)
- **K** = constante que depende do material do condutor e do isolamento

**Valores de K para condutores de proteção:**

Material do condutorIsolamento PVCIsolamento XLPE/EPRCobre115143Alumínio7694Aço4252
**Exemplo de cálculo:** circuito com corrente de falta Icc = 2.000 A, disjuntor com tempo de atuação t = 0,1 s, condutor de cobre com isolamento PVC:

S = √(2.000² × 0,1) / 115

S = √(400.000) / 115

S = 632,5 / 115

S = 5,5 mm²

Neste caso, o PE mínimo seria 6 mm². Se a tabela simplificada indicasse 10 mm² (para fase de 10 mm²), o projetista pode justificar a redução para 6 mm² pelo cálculo térmico — desde que documentado no projeto.

A fórmula adiabática é especialmente útil em instalações industriais de grande porte, onde a diferença entre o resultado da tabela e o cálculo pode representar economia significativa em cobre.

### PE em eletroduto metálico e eletrocalha

A NBR 5410 permite que eletrodutos metálicos e eletrocalhas sirvam como condutor de proteção, desde que:

- A continuidade elétrica seja garantida ao longo de todo o percurso
- As conexões (luvas, buchas, niples) assegurem contato permanente e de baixa resistência
- A seção transversal da parede metálica atenda ao dimensionamento mínimo

Na prática, essa opção é mais comum em instalações industriais com eletrodutos de aço galvanizado pesado. Em instalações residenciais e comerciais, o PE é sempre um condutor isolado instalado junto com os condutores fase e neutro.

### Identificação por cores

A normalização de cores pela NBR 5410 é taxativa:

CondutorCor obrigatóriaObservaçãoPE (proteção)Verde-amarelo (bicolor)Exclusiva — nenhum outro condutor pode usarPEN (proteção + neutro)Azul-claro com indicação verde-amarelo nas extremidadesSomente em esquema TN-CNeutro (N)Azul-claroExclusiva para neutroFaseQualquer cor exceto verde-amarelo, azul-claro e verdePreto, vermelho e branco são as mais comuns
A cor verde (isolada, sem amarelo) não é prevista na NBR 5410 para o PE — a norma especifica bicolor verde-amarelo. Na prática brasileira, cabos verdes são encontrados em instalações antigas, mas não atendem à nomenclatura normativa atual.

### Diferença entre PE, PEN e condutor de aterramento

Três condutores que frequentemente geram confusão:

**PE (Protective Earth):** conecta as massas ao aterramento. Presente em todos os esquemas de aterramento. Conduz corrente apenas em situação de falta.

**PEN (Protective Earth + Neutral):** condutor que acumula as funções de PE e neutro. Existe apenas no esquema TN-C. Conduz corrente de neutro (desequilíbrio) em operação normal. Por isso, o PEN nunca pode ser seccionado unilateralmente e sua seção mínima é 10 mm² (cobre) ou 16 mm² (alumínio), independentemente do resultado da tabela.

**Condutor de aterramento:** conecta o [BEP](/bep-barramento-equipotencializacao) ao eletrodo de aterramento (haste, malha, ferragem). Não é o PE — é o trecho entre o barramento e o solo. Sua seção mínima depende do esquema de aterramento e do sistema de proteção contra descargas atmosféricas.

Nos [sistemas TT, TN e IT](/sistemas-tt-tn-it-diferencas), o papel do PE varia: no TT, o PE conecta as massas a um aterramento independente da concessionária; no TN, o PE (ou PEN) conduz a corrente de falta de volta ao transformador.

### Condutor de equipotencialização

Além do PE dos circuitos, a NBR 5410 exige condutores de equipotencialização que interligam ao BEP:

- Tubulações metálicas (água, gás, esgoto)
- Estrutura metálica da edificação
- Armaduras de concreto armado
- Blindagem de cabos
- Eletrodutos metálicos

A seção mínima do condutor de equipotencialização principal é 6 mm² (cobre) ou equivalente. Já o condutor de equipotencialização suplementar (entre duas massas ou entre massa e elemento condutor estranho) deve ter seção não inferior à do menor PE conectado a essas massas.

### Erros frequentes no dimensionamento do PE

**1. Usar PE inferior à fase em circuitos ≤ 16 mm²**

Para fase de 2,5 mm², o PE deve ser 2,5 mm² — não 1,5 mm². A tabela é clara: até 16 mm², o PE é igual à fase.

**2. Eliminar o PE em circuitos de iluminação**

A NBR 5410 exige PE em todos os circuitos, incluindo iluminação. Luminárias metálicas sem PE são ponto de falha com risco de choque.

**3. Usar o neutro como PE**

Neutro e PE têm funções distintas. Conectá-los no ponto errado (fora do BEP/quadro de entrada) cria circulação de corrente pelo PE, elevando o potencial das massas. Essa prática é proibida no [esquema TN-S](/sistemas-tt-tn-it-diferencas).

**4. Não instalar PE nos circuitos de ar-condicionado split**

O circuito do condensador (unidade externa) exige PE — a carcaça metálica está exposta a intempéries e toque humano.

**5. Seccionar o PEN sem converter para TN-C-S**

O PEN só pode ser dividido em PE + N no ponto de transição TN-C para TN-S (tipicamente no quadro de entrada). A partir desse ponto, PE e N seguem separados e nunca mais são reconectados.

### Verificação em campo

Após a instalação, a verificação do PE inclui:

- **Continuidade:** medição com ohmímetro de baixa resistência ( 35 → PE = S/2) é o método padrão. O cálculo adiabático S = √(I²t)/K permite otimização quando justificado tecnicamente. O PE deve ser verde-amarelo, presente em todos os circuitos, e nunca confundido com o neutro. Um PE corretamente dimensionado e instalado é a diferença entre um defeito que desliga o disjuntor e um defeito que causa [choque elétrico letal](/tensao-passo-toque-protecao-pessoas).

### Links relacionados

- → S1: Diferença entre Terra, Neutro e Massa (`/diferenca-terra-neutro-massa`)
- → PILAR: Guia Completo de Aterramento (`/aterramento-eletrico-guia-completo`)
- → S7: BEP (`/bep-barramento-equipotencializacao`)
- → S2: Sistemas TT, TN e IT (`/sistemas-tt-tn-it-diferencas`)
- → S6: Tensão de Passo e Toque (`/tensao-passo-toque-protecao-pessoas`)

Dúvida no dimensionamento do condutor PE ou na configuração do sistema de proteção? A equipe AEOMaps revisa o projeto e garante conformidade com a NBR 5410.

**[Fale com um especialista pelo WhatsApp →](https://wa.me/5511925222281?text=Olá!%20Vim%20pelo%20artigo%20sobre%20condutor%20de%20proteção%20PE%20e%20preciso%20de%20orientação%20técnica.)**