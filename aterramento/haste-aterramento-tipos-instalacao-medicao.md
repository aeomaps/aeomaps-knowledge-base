---
title: "Haste de Aterramento: Tipos, Instalação e Medição com Terrômetro"
slug: haste-aterramento-tipos-instalacao-medicao
date: 2026-06-03 10:00:00
categories: Aterramento
tags: copperweld, eletrodo, haste de aterramento, medição, NBR 15749, resistência, solda exotérmica, terrômetro
source: aeomaps.com.br/haste-aterramento-tipos-instalacao-medicao/
---

### Função da haste no sistema de aterramento

A haste de aterramento é o elemento mais comum de contato entre a instalação elétrica e o solo. Sua função é estabelecer um caminho de baixa impedância para correntes de falta e descargas atmosféricas, permitindo o escoamento seguro para o solo.

Porém, a haste é apenas um componente do sistema de aterramento — não é o sistema completo. A NBR 5419:2026 deixou isso explícito: a haste isolada não é reconhecida como eletrodo protagonista do SPDA. A norma exige eletrodo em anel como configuração mínima, podendo ser complementado com hastes verticais.

Para instalações de baixa tensão (NBR 5410), a haste continua sendo o eletrodo mais utilizado em instalações residenciais e comerciais de pequeno porte.

### Tipos de haste disponíveis no mercado brasileiro

**Haste copperweld (aço revestido de cobre):**

É o padrão brasileiro. Consiste em uma alma de aço carbono revestida por camada de cobre eletrodepositado. O aço fornece resistência mecânica para cravação; o cobre garante baixa resistividade e resistência à corrosão.

Dimensões comerciais mais comuns:

DiâmetroComprimentoAplicação típica1/2" (12,7 mm)2,40 mResidencial, comercial pequeno5/8" (15,9 mm)2,40 mComercial, industrial leve3/4" (19,0 mm)3,00 mIndustrial, SPDA
A espessura mínima de cobre deve ser de 254 μm (0,254 mm) para garantir proteção contra corrosão. Hastes com revestimento inferior apresentam degradação acelerada, especialmente em solos ácidos.

**Haste de aço inoxidável:**

Utilizada em solos com alta agressividade química (salinidade, pH extremo). Custo mais elevado. Não sofre corrosão galvânica com condutores de cobre.

**Haste de cobre maciço:**

Rara no Brasil por custo. Sem problemas de continuidade do revestimento, mas com menor resistência mecânica para cravação em solos duros.

### Cravação: profundidade e técnica

A haste deve ser cravada verticalmente até que apenas 10 a 20 cm fiquem acima do solo (para conexão do condutor). Em solos com camada superficial resistiva e camada profunda condutiva, a cravação total maximiza o contato com o estrato mais condutivo.

Regras práticas de cravação:

- A distância entre hastes em paralelo deve ser pelo menos igual ao comprimento da haste (regra d ≥ L). Hastes muito próximas interferem mutuamente e a redução de resistência é inferior à esperada.
- Em solos rochosos onde a cravação vertical é impossível, a alternativa é instalação inclinada (45°) ou complementação horizontal com cabo nu enterrado.
- A cravação pode ser manual (marreta com cabeçote de proteção) ou mecânica (martelete pneumático ou hidráulico).
- Nunca cortar a haste para reduzir o comprimento — a redução de comprimento aumenta a resistência proporcionalmente.

### Conexões: solda exotérmica vs conectores mecânicos

A conexão entre a haste e o condutor de aterramento é ponto crítico de continuidade. Existem dois métodos principais:

**Solda exotérmica (Cadweld, Burndy, similares):**

Reação aluminotérmica que funde o condutor e a haste em uma conexão molecular permanente. Vantagens:

- Resistência mecânica superior à do próprio condutor
- Resistência elétrica da junta inferior à do condutor
- Imune a afrouxamento por vibração ou dilatação térmica
- Resistência à corrosão superior ao conector mecânico

Requer moldes específicos para cada combinação haste/condutor e mão de obra capacitada.

**Conector mecânico (parafuso):**

Mais rápido e barato, mas sujeito a afrouxamento, corrosão na interface e aumento de resistência ao longo do tempo. Aceitável em instalações temporárias ou quando a solda exotérmica não é viável. Exige inspeção periódica.

Para instalações permanentes e SPDA, a solda exotérmica é a prática recomendada.

### Fórmula de resistência de uma haste vertical

A resistência de aterramento de uma haste vertical cravada em solo homogêneo é calculada pela fórmula de Sunde & Dwight:

**R = ρ / (2πL) × [ln(4L/a) − 1]**

Onde:

- R = resistência de aterramento (Ω)
- ρ = [resistividade do solo](/resistividade-solo-metodo-wenner) (Ω·m)
- L = comprimento da haste enterrado (m)
- a = raio da haste (m)
- ln = logaritmo natural

Exemplo prático: haste copperweld 5/8" (a = 0,008 m), L = 2,40 m, solo argiloso ρ = 100 Ω·m:

R = 100 / (2π × 2,40) × [ln(4 × 2,40 / 0,008) − 1]

R = 6,63 × [ln(1.200) − 1]

R = 6,63 × [7,09 − 1]

R = 6,63 × 6,09

R ≈ 40,4 Ω

Para o mesmo solo, com haste de 3,00 m:

R = 100 / (2π × 3,00) × [ln(4 × 3,00 / 0,008) − 1]

R = 5,31 × [ln(1.500) − 1]

R = 5,31 × [7,31 − 1]

R = 5,31 × 6,31

R ≈ 33,5 Ω

A aproximação simplificada de Sunde é útil para estimativas rápidas:

**R ≈ ρ / L**

Para ρ = 100 Ω·m e L = 2,40 m: R ≈ 41,7 Ω — valor compatível com o cálculo completo.

### Hastes em paralelo

Quando uma haste única não atinge a resistência desejada, a solução é instalar [hastes em paralelo](/como-reduzir-resistencia-aterramento). A resistência do conjunto é menor que a de cada haste individual, mas não se divide linearmente.

Regra prática:

- 2 hastes (d ≥ L): R_conjunto ≈ R_individual × 0,58
- 3 hastes em triângulo (d ≥ L): R_conjunto ≈ R_individual × 0,43
- 4 hastes em quadrado (d ≥ L): R_conjunto ≈ R_individual × 0,35

Se a distância entre hastes for menor que o comprimento (d Seção fase (mm²)PE mínimo (mm²)S ≤ 16S16 < S ≤ 3516S > 35S/2
### Conclusão técnica

A haste de aterramento é o componente mais acessível do sistema de aterramento, mas seu desempenho depende do tipo de solo, da profundidade de cravação, da qualidade da conexão e da geometria do arranjo. A medição com terrômetro pelo método de queda de potencial (NBR 15749) é o único procedimento válido para determinação da resistência em laudos técnicos.

A NBR 5419:2026 exige anel como eletrodo principal — hastes são complementares.

### Links relacionados

- [Como Reduzir a Resistência de Aterramento](/como-reduzir-resistencia-aterramento) — hastes em paralelo, tratamento, ferragem
- [Resistividade do Solo — Método de Wenner](/resistividade-solo-metodo-wenner) — dado de entrada para dimensionamento de hastes
- [O Mito dos 10Ω](/mito-10-ohms-resistencia-aterramento) — valor correto de resistência conforme o esquema
- [Guia Completo de Aterramento](/aterramento-eletrico-guia-completo) — visão geral do sistema

Precisa dimensionar hastes, escolher o tipo certo ou validar a medição com terrômetro? A equipe AEOMaps orienta desde a seleção do eletrodo até a interpretação dos resultados.

**[Fale com um especialista pelo WhatsApp →](https://wa.me/5511925222281?text=Olá!%20Vim%20pelo%20artigo%20sobre%20haste%20de%20aterramento%20e%20preciso%20de%20orientação%20técnica.)**