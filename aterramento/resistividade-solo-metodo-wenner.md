---
title: "Resistividade do Solo: Como Medir pelo Método de Wenner (NBR 7117)"
slug: resistividade-solo-metodo-wenner
date: 2026-06-04 08:00:00
categories: Aterramento
tags: aterramento, estratificação, medição, NBR 7117, resistividade, solo, tabela, Wenner
source: aeomaps.com.br/resistividade-solo-metodo-wenner/
---

### O que é resistividade do solo e por que medir

Resistividade elétrica do solo (ρ) é a propriedade que define a oposição do solo à passagem de corrente elétrica. É medida em ohm-metro (Ω·m) e varia de 5 Ω·m (pântano) a mais de 10.000 Ω·m (basalto seco).

A resistividade é o dado de entrada fundamental para o dimensionamento de qualquer sistema de aterramento. Sem essa medição, o projetista trabalha às cegas — pode sobredimensionar (custo desnecessário) ou subdimensionar (não conformidade normativa e risco).

A resistividade determina diretamente a resistência do eletrodo de aterramento: para uma haste vertical, a aproximação simplificada é R ≈ ρ/L. Em solo de 100 Ω·m, uma haste de 2,40 m terá R ≈ 42 Ω. Em solo de 1.000 Ω·m, a mesma haste terá R ≈ 417 Ω.

### Fatores que influenciam a resistividade

A resistividade do solo não é constante — varia com composição mineralógica, umidade, salinidade, temperatura e compactação.

**Variação com umidade (solo arenoso-argiloso):**

Umidade (% peso)ρ (Ω·m)0%10.0002,5%1.5005%43010%18515%10520%6330%42
A resistividade cai drasticamente entre 0% e 10% de umidade — uma variação de 50× . Acima de 15%, a redução é mais gradual. Isso explica por que a resistência de aterramento varia com as estações: em períodos secos, a resistividade aumenta significativamente.

**Variação com salinidade:**

Sal (% peso)ρ (Ω·m)0%1070,1%181%4,65%1,910%1,320%1,0
Sais dissolvidos na água intersticial são os principais responsáveis pela condutividade do solo. Apenas 0,1% de sal reduz a resistividade em 6×.

**Variação com temperatura:**

Temperatura (°C)ρ (Ω·m)207210990 (água)1380 (gelo)300−5790−73.300
O congelamento da água nos poros do solo aumenta a resistividade drasticamente. Em regiões sujeitas a geada, a resistência de aterramento pode subir 10× ou mais no inverno.

### Tabela de resistividade por tipo de solo

Tipo de soloMín (Ω·m)Médio (Ω·m)Máx (Ω·m)Pântano, charcos, terra com húmus530100Solo arado, barro e argila80100500Argila arenosa50150500Argila com 40% umidade—80—Argila com 20% umidade—330—Argila seca1.500—5.000Terra de jardim 50% umidade—140—Terra de jardim 20% umidade—480—Solo arenoso 90% umidade2008001.000Solo arenoso seco—1.300—Areia (molhada a seca)5001.0008.000Calcário compacto1.000—8.000Calcário fissurado5001.0008.000Granito1.500—10.000Basalto10.000—20.000
Esses valores são referências gerais. A resistividade real do terreno específico deve ser medida em campo — usar a tabela como substituto da medição é erro de projeto.

### Método de Wenner: princípio e procedimento

O método de Wenner (ou método dos quatro eletrodos) é o procedimento padronizado pela NBR 7117:2020 para medição de resistividade do solo. Utiliza quatro hastes equidistantes cravadas em linha reta na superfície do solo.

**Arranjo:**

Quatro hastes (A, M, N, B) são cravadas em linha, com espaçamento igual "a" entre cada uma. O instrumento injeta corrente entre as hastes externas (A e B) e mede a tensão entre as hastes internas (M e N).

**Fórmula:**

**ρ = 2πaR**

Onde:

- ρ = resistividade aparente do solo (Ω·m)
- a = espaçamento entre hastes (m)
- R = resistência lida no instrumento (Ω)

A resistividade obtida é chamada "aparente" porque representa uma média ponderada das camadas de solo até uma profundidade aproximadamente igual ao espaçamento "a". Quanto maior o espaçamento, mais profundas são as camadas que influenciam a medição.

### Procedimento de campo detalhado

**Equipamento necessário:**

- Terrômetro de 4 terminais (medidor de resistividade)
- 4 hastes auxiliares de aço galvanizado (diâmetro 10-15 mm, comprimento 50 cm)
- Trena ou corda com marcações nos espaçamentos
- Marreta leve
- Planilha de campo

**Sequência de medição:**

- Definir a linha de medição no terreno. Preferencialmente em área representativa do local onde será instalado o eletrodo de aterramento.

- Cravar as 4 hastes em linha reta, alinhadas e equidistantes, com profundidade de cravação de 20-30 cm (máximo 10% do espaçamento "a").

- Medir com os seguintes espaçamentos progressivos: 1, 2, 4, 8, 16, 32 e 64 metros. Cada espaçamento revela a resistividade de uma camada mais profunda.

- Registrar a leitura R do instrumento para cada espaçamento.

- Calcular ρ = 2πaR para cada espaçamento.

- Repetir a medição em no mínimo 3 direções diferentes, com ângulos de 60° entre elas. Essa prática identifica heterogeneidades laterais do solo.

- Para cada espaçamento, verificar a dispersão entre as direções. Se a variação entre medições de um mesmo espaçamento exceder 50%, investigar a causa (tubulação metálica, rocha, aterro) e considerar medições adicionais.

### Tratamento dos dados: curva ρ × a

Os valores de resistividade aparente são plotados em gráfico com escalas bilogarítmicas: espaçamento "a" no eixo horizontal e resistividade ρ no eixo vertical.

O formato da curva revela a estrutura do solo:

- **Curva descendente:** camada superior mais resistiva que a inferior (caso favorável para hastes profundas)
- **Curva ascendente:** camada superior menos resistiva que a inferior (hastes profundas terão menor eficácia)
- **Curva com mínimo:** solo estratificado com camada condutora intermediária
- **Curva constante:** solo homogêneo (raro na prática)

### Estratificação do solo

A NBR 7117:2020 exige que os dados de medição sejam interpretados para determinação do modelo de camadas do solo. O modelo mais comum é o de duas camadas:

- ρ₁ = resistividade da primeira camada (superficial)
- h₁ = espessura da primeira camada
- ρ₂ = resistividade da segunda camada (profunda)

A determinação dos parâmetros pode ser feita por métodos gráficos (curvas de Sunde, ábacos) ou por software de inversão (RESAP, AGE, AutoGrid Pro).

Exemplo real — laudo em Curitiba (8 linhas de medição):

- Camada 1: ρ₁ = 105,6 Ω·m
- Camada 2: ρ₂ = 39,12 Ω·m

Nesse caso, a camada profunda é mais condutiva — [hastes longas](/haste-aterramento-tipos-instalacao-medicao) são favoráveis.

### Erros comuns na medição

**Cravação excessiva das hastes auxiliares:** se a profundidade de cravação exceder 10% do espaçamento "a", a medição é distorcida. Para espaçamento de 1 m, a cravação máxima é 10 cm.

**Hastes desalinhadas:** desvio significativo da linha reta entre as hastes altera a geometria do campo elétrico e invalida a fórmula ρ = 2πaR.

**Proximidade de estruturas metálicas:** tubulações, cercas, ferragens e cabos enterrados desviam a corrente e produzem valores artificialmente baixos.

**Medição após chuva intensa:** a saturação temporária do solo fornece valores otimistas que não representam a condição de seca. O ideal é medir em período representativo ou aplicar fatores de correção sazonal.

**Usar apenas uma direção:** uma única linha pode passar sobre uma anomalia (rocha, aterro, tubulação) sem que o operador perceba. Três direções a 60° são o mínimo.

### Quando a medição é obrigatória

A prospecção de resistividade é obrigatória ou fortemente recomendada em:

- Projetos de SPDA (NBR 5419)
- Instalações industriais de médio e grande porte
- Subestações (IEEE Std 80)
- Torres de telecomunicação
- Sistemas fotovoltaicos de grande porte

Em instalações residenciais, a medição nem sempre é exigida formalmente, mas é a única forma de dimensionar corretamente o aterramento sem sobredimensionamento.

### Conclusão técnica

A resistividade do solo é o dado de entrada insubstituível para o dimensionamento do aterramento. O método de Wenner (NBR 7117:2020) com quatro hastes equidistantes, medição em 3+ direções e espaçamentos progressivos é o procedimento padronizado. A curva ρ × a em papel bilogarítmico revela a estratificação do solo e orienta a escolha entre hastes profundas, cabos horizontais, malha ou [tratamento químico](/como-reduzir-resistencia-aterramento).

### Links relacionados

- [Haste de Aterramento](/haste-aterramento-tipos-instalacao-medicao) — dimensionamento a partir da resistividade medida
- [Como Reduzir a Resistência de Aterramento](/como-reduzir-resistencia-aterramento) — quando a resistividade é alta
- [Aterramento em Solo Rochoso](/aterramento-solo-rochoso-solucoes) — soluções para altíssima resistividade
- [Guia Completo de Aterramento](/aterramento-eletrico-guia-completo) — visão geral do sistema
- [Custos de Aterramento](/custo-sistema-aterramento) — impacto da resistividade no custo

Precisa de ensaio de resistividade do solo ou projeto de aterramento baseado em dados reais de campo? A equipe AEOMaps executa prospecção com Wenner e interpreta a estratificação para dimensionar o sistema correto.

**[Fale com um especialista pelo WhatsApp →](https://wa.me/5511925222281?text=Olá!%20Vim%20pelo%20artigo%20sobre%20resistividade%20do%20solo%20e%20preciso%20de%20orientação%20técnica.)**