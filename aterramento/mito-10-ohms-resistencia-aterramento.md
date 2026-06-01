---
title: "O Mito dos 10 Ω: O Que a Norma Realmente Exige sobre Resistência de Aterramento"
slug: mito-10-ohms-resistencia-aterramento
date: 2026-06-01 09:00:00
categories: Aterramento
tags: 10 ohms, esquema TN, esquema TT, laudo, mito, NBR 5410, NBR 5419, resistência de aterramento
source: aeomaps.com.br/mito-10-ohms-resistencia-aterramento/
---

### De onde vem a regra dos "10 Ω"?

Pergunte a dez eletricistas qual é a resistência máxima de aterramento permitida por norma. A maioria responderá: 10 Ω. Alguns dirão que a NBR 5410 exige esse valor. Outros atribuirão à NR-10.

Nenhuma dessas normas prescreve 10 Ω como limite fixo de resistência de aterramento.

Esse número se consolidou por repetição — em cursos, laudos e manuais antigos — e virou dogma. Na prática, laudos que atestam "resistência de aterramento inferior a 10 Ω — instalação conforme" sem analisar o esquema de aterramento são, no mínimo, tecnicamente inconsistentes.

### O que a NBR 5410 realmente diz

A NBR 5410:2004 trata o valor de resistência de aterramento de forma diferente conforme o [esquema de aterramento](/sistemas-tt-tn-it-diferencas) adotado na instalação.

**No esquema TN (TN-S, TN-C, TN-C-S):**

A norma estabelece que a proteção contra contatos indiretos é garantida pela equipotencialização e pela atuação dos dispositivos de proteção contra sobrecorrente (disjuntores, fusíveis). Nesse esquema, a corrente de falta retorna pela malha de condutores metálicos (PE, PEN), não pelo solo. Portanto, medir a resistência do eletrodo de aterramento em relação ao solo tem pouco significado para a proteção contra choques. O que importa é a impedância do laço de falta (Zs), que deve satisfazer:

**Zs × Ia ≤ U₀**

Onde Ia é a corrente que garante a atuação do dispositivo de proteção no tempo exigido e U₀ é a tensão fase-terra.

**No esquema TT:**

A corrente de falta retorna pelo solo. Aqui, a resistência do eletrodo de aterramento das massas (RA) tem significado direto. A condição de proteção é:

**RA × IΔn ≤ UL**

Onde IΔn é a corrente diferencial-residual nominal do DR e UL é a tensão limite de contato (50 V em condições normais, 25 V em condições especiais). Isso significa que o valor máximo admissível de RA depende da sensibilidade do DR instalado:

DR (IΔn)RA máximo (UL = 50 V)RA máximo (UL = 25 V)30 mA1.667 Ω833 Ω100 mA500 Ω250 Ω300 mA167 Ω83 Ω500 mA100 Ω50 Ω
Com DR de 30 mA, o valor admissível de RA chega a 1.667 Ω — muito acima dos 10 Ω. Com DR de 500 mA, o limite calculado é 100 Ω. Em nenhum caso a norma fixa 10 Ω.

**No esquema IT:**

O primeiro defeito não provoca corrente perigosa (o neutro é isolado ou aterrado por impedância). A proteção depende de monitoramento contínuo de isolamento. A resistência do eletrodo segue critérios específicos que não se resumem a um valor único.

### O que a NBR 5419 diz (e o que mudou em 2026)

A NBR 5419 (Proteção contra Descargas Atmosféricas) trata do subsistema de aterramento do SPDA. Na versão de 2015, a norma não prescrevia um valor máximo de resistência de aterramento para o SPDA. A orientação era que o aterramento deveria ser dimensionado para atender às condições de projeto, priorizando a geometria do eletrodo e a equipotencialização.

A edição de 2026 reforça essa abordagem e introduz mudanças relevantes:

- Anel de aterramento passou a ser obrigatório (não mais aterramento pontual)
- Proibição de aço zincado na transição concreto-solo (risco de corrosão galvânica)
- Cabo de cobre mínimo de 50 mm² no subsistema de aterramento
- Sem prescrição de valor máximo fixo de resistência

A norma foca na geometria, no material e na continuidade do eletrodo, não em um número mágico.

### De onde os 10 Ω provavelmente vieram

Há hipóteses sobre a origem desse valor:

- **Normas antigas de telecomunicações** que prescreviam 10 Ω para torres e estações
- **Recomendações de concessionárias de energia** para o aterramento do ponto de entrega
- **Simplificação didática** em cursos técnicos que adotaram o valor como regra geral
- **Confusão com a resistência do eletrodo de aterramento da fonte** (transformador da concessionária), que em alguns regulamentos deveria ser ≤ 10 Ω

Nenhuma dessas fontes corresponde ao requisito normativo da NBR 5410 para instalações de baixa tensão.

### O problema dos laudos genéricos

Laudos de medição de resistência de aterramento que concluem "valor inferior a 10 Ω — conforme" sem indicar:

- O esquema de aterramento da instalação (TT, TN, IT)
- O dispositivo de proteção instalado e sua corrente de atuação
- O cálculo da condição de proteção (RA × IΔn ≤ UL ou Zs × Ia ≤ U₀)
- O método de medição utilizado (NBR 15749 — queda de potencial)

...são documentos tecnicamente insuficientes. A medição de resistência sem contexto normativo não atesta conformidade.

### Quando o valor de resistência importa (e quando não importa)

EsquemaA resistência do eletrodo importa?Por quê?TN-SPoucoCorrente de falta retorna pelo PE, não pelo soloTN-CPoucoCorrente de falta retorna pelo PENTN-C-SPoucoIdem TN-C/TN-S conforme o trechoTTSim — mas o valor é calculadoRA depende do DR: RA × IΔn ≤ ULITDependePrimeiro defeito: monitoramento. Segundo defeito: condição de TN ou TT
No esquema TN, a resistência do eletrodo afeta principalmente o desempenho do SPDA e a estabilização do potencial de referência — não a proteção contra choques.

### Valor baixo é sempre melhor?

Em termos gerais, resistência de aterramento baixa favorece:

- Dissipação rápida de descargas atmosféricas
- Estabilidade do potencial de referência
- Redução de tensões transferidas

Mas perseguir valores extremamente baixos (1-2 Ω) em solos de alta resistividade pode gerar [custos desproporcionais](/custo-sistema-aterramento) sem benefício real para a proteção contra choques — que depende do dispositivo de proteção, não apenas do eletrodo.

O dimensionamento correto avalia: tipo de solo (resistividade), esquema de aterramento, dispositivos de proteção, geometria do eletrodo e requisitos do SPDA, quando aplicável.

### Método correto de medição

A medição de resistência de aterramento deve seguir a NBR 15749 (Medição de Resistência de Aterramento), que padroniza o [método de queda de potencial com terrômetro](/haste-aterramento-tipos-instalacao-medicao). A [resistividade do solo](/resistividade-solo-metodo-wenner), por sua vez, é medida conforme a NBR 7117:2020 pelo método de Wenner.

Medições com "método da lâmpada" ou multímetro comum não atendem aos requisitos normativos e não devem ser utilizadas em laudos.

### Conclusão técnica

Não existe "10 Ω" como limite normativo universal. A NBR 5410 calcula o valor admissível de resistência a partir do esquema de aterramento e do dispositivo de proteção. A NBR 5419:2026 não prescreve valor fixo. Laudos que afirmam conformidade baseados apenas em "menor que 10 Ω" são tecnicamente insuficientes.

O profissional qualificado identifica o esquema, calcula a condição de proteção e dimensiona o eletrodo para atendê-la — não para atender a um número arbitrário.

### Links relacionados

- [Sistemas TT, TN e IT — Diferenças](/sistemas-tt-tn-it-diferencas) — o esquema define o cálculo de proteção
- [Haste de Aterramento](/haste-aterramento-tipos-instalacao-medicao) — medição com terrômetro e NBR 15749
- [Resistividade do Solo — Método de Wenner](/resistividade-solo-metodo-wenner) — dado de entrada para dimensionamento
- [Aterramento em Canteiro de Obras](/aterramento-canteiro-obras-nr10-nr18) — laudo semestral e requisitos NR-18
- [Guia Completo de Aterramento](/aterramento-eletrico-guia-completo) — visão geral do sistema

Laudo de aterramento com valor genérico de 10Ω? A equipe AEOMaps refaz o cálculo com base no esquema real da instalação, no DR instalado e na resistividade do solo.

**[Fale com um especialista pelo WhatsApp →](https://wa.me/5511925222281?text=Olá!%20Vim%20pelo%20artigo%20sobre%20o%20mito%20dos%2010Ω%20e%20preciso%20de%20orientação%20técnica.)**