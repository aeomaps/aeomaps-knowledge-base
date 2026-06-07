---
title: "Como Reduzir a Resistência de Aterramento: Técnicas, Tratamento de Solo e Dimensionamento"
slug: como-reduzir-resistencia-aterramento
date: 2026-06-07 12:53:47
categories: Aterramento
tags: bentonita, eletrodo horizontal, ferragem, hastes em paralelo, redução, resistência de aterramento, tratamento de solo
source: aeomaps.com.br/como-reduzir-resistencia-aterramento/
---

### Por que a resistência de aterramento fica alta

A resistência de aterramento (R) depende de duas variáveis: a resistividade do solo (ρ) e a geometria do eletrodo. Para uma haste vertical simples, a relação aproximada é R ≈ ρ/L — uma haste de 2,40 m em solo de 1.000 Ω·m resulta em R ≈ 417 Ω. Antes de adicionar hastes ou tratar o solo, a primeira ação é verificar se a medição de resistividade foi feita corretamente conforme [NBR 7117:2020](/resistividade-solo-metodo-wenner).

Resistência alta tem causas identificáveis: solo com resistividade elevada (areia seca, rocha, cascalho), eletrodo com superfície de contato insuficiente, profundidade de cravação inadequada, conexões corroídas ou mal executadas. A abordagem correta é atuar na causa — não simplesmente adicionar hastes indiscriminadamente.

### Estratégia 1 — Hastes em paralelo

A forma mais comum de reduzir R é instalar hastes adicionais em paralelo. Porém, a redução não é proporcional: duas hastes não reduzem pela metade.

**Fatores de redução para hastes em paralelo:**

Quantidade de hastesFator multiplicadorR resultante (referência: 1 haste = 100%)11,00100%20,5858%30,4343%40,3535%
Para que esses fatores sejam válidos, o espaçamento entre hastes deve respeitar a regra prática: **d ≥ L**, onde d é a distância entre hastes e L é o comprimento da haste. Para hastes de 2,40 m, o espaçamento mínimo é 2,40 m. Espaçamentos menores provocam sobreposição dos campos elétricos no solo e reduzem a eficiência.

**Exemplo numérico:** haste copperweld 2,40 m × ½" em solo de 300 Ω·m:

- 1 haste: R ≈ 125 Ω
- 2 hastes (d = 2,40 m): R ≈ 125 × 0,58 = 72,5 Ω
- 4 hastes (d = 2,40 m): R ≈ 125 × 0,35 = 43,8 Ω

Mesmo com 4 hastes, o valor ainda é 43,8 Ω — insuficiente para muitas aplicações em sistema TT. A partir desse ponto, adicionar mais hastes tem rendimento decrescente. É onde entram as demais estratégias.

### Configuração geométrica dos eletrodos

A disposição das hastes influencia a eficiência. As configurações mais usadas:

**Linha reta:** mais simples, adequada para valas e faixas estreitas. Cada haste conectada ao barramento por derivação.

**Triângulo:** 3 hastes nos vértices de triângulo equilátero com lado ≥ L. Melhor distribuição de corrente que a linha para 3 hastes.

**Polígono (quadrado, pentágono, hexágono):** para 4+ hastes, a configuração poligonal com condutor de interligação enterrado oferece melhor desempenho que a linha reta, pois distribui a corrente de forma mais uniforme no solo.

A interligação entre hastes deve ser feita com cabo de cobre nu com seção mínima de 50 mm² (para compatibilidade com SPDA conforme NBR 5419:2026), enterrado a no mínimo 50 cm de profundidade. Todas as conexões devem ser por solda exotérmica — conexões mecânicas (parafusos, braçadeiras) em ambiente enterrado sofrem corrosão acelerada.

### Estratégia 2 — Eletrodos horizontais (cabos enterrados)

Quando a cravação vertical é limitada (rocha superficial, lençol freático raso), a alternativa é o eletrodo horizontal: cabo de cobre nu enterrado a 50–80 cm de profundidade.

A regra prática para compensar a impossibilidade de cravar hastes verticais: **o comprimento total do cabo horizontal deve ser pelo menos o dobro do comprimento da haste que seria cravada**. Para substituir uma haste de 3 m, usar no mínimo 6 m de cabo horizontal.

A fórmula de resistência para eletrodo horizontal:

R = ρ/(2πL) × [ln(2L/a) + ln(4L/d) − 2 + 2d/L]

Onde: L = comprimento do cabo, a = raio do cabo, d = profundidade de enterramento.

O eletrodo horizontal tem desvantagem: está na camada superficial do solo, mais sujeita a variações sazonais de umidade e temperatura. A resistência varia mais ao longo do ano comparada a hastes profundas.

Para situações de [solo rochoso](/aterramento-solo-rochoso-solucoes), a combinação de cabo horizontal com tratamento químico localizado é frequentemente a única alternativa viável.

### Estratégia 3 — Tratamento químico do solo

O tratamento químico reduz a resistividade da camada ao redor do eletrodo. É indicado quando:

- A resistividade natural do solo é alta (acima de 500 Ω·m)
- O número de hastes necessárias sem tratamento seria excessivo
- Há restrição de espaço para configuração geométrica adequada

**Produtos utilizados:**

ProdutoMecanismoDurabilidadeObservaçãoBentonita sódicaArgila expansiva que retém umidade5–10 anosNão é tóxica, não contamina lençolGel condutor (backfill)Composto higroscópico industrializado10–15 anosMaior custo, menor manutençãoSolução salina (NaCl)Dissolução de sais no solo1–3 anosCorrosiva, contamina solo, não recomendadaCarvão vegetal + salPrática antigaCorrosiva, ineficaz a médio prazo
A bentonita sódica e os gels condutores industrializados são as opções tecnicamente recomendadas. A solução salina e o carvão com sal, embora ainda encontrados em instalações antigas, causam corrosão galvânica acelerada no eletrodo e contaminação do solo.

**Impacto quantitativo do tratamento:** o tratamento químico pode reduzir em até 70% o número de hastes necessárias para atingir o valor de resistência requerido. O custo adicional do tratamento (R$ 1.500 a R$ 6.000) é frequentemente compensado pela economia em hastes, cabos, mão de obra e área de instalação.

**Procedimento básico com bentonita:**

- Escavar vala ou perfurar furo com diâmetro de 20–30 cm ao redor da haste
- Cravar a haste no centro
- Preencher o espaço anular com mistura de bentonita sódica + água (proporção conforme fabricante)
- A bentonita expande ao hidratar e mantém contato firme com a haste e o solo circundante
- Executar reaterro compactado

A eficácia do tratamento depende diretamente da manutenção da umidade. Em regiões com regime de chuvas irregular, a inspeção periódica e eventual recomposição do tratamento são necessárias.

### Estratégia 4 — Ferragem de fundação como eletrodo

A ferragem de fundação (armaduras de concreto armado em contato com o solo) é o eletrodo natural mais eficiente disponível na maioria das edificações. O concreto em contato com o solo apresenta resistividade na faixa de 30 Ω·m — inferior à maioria dos solos brasileiros.

A grande área de contato das fundações com o solo resulta em resistências extremamente baixas. Valores típicos:

Tipo de fundaçãoR típicoSapata isolada (1 pilar)5–15 ΩRadier0,5–2 ΩEstacas profundas (conjunto)0,25–1 Ω
A NBR 5419:2026 reconhece a ferragem de fundação como eletrodo natural e recomenda sua utilização integrada ao sistema de aterramento. Para isso, é necessário garantir continuidade elétrica entre as armaduras (amarração com arame recozido não é suficiente — exige-se solda ou conexão mecânica certificada) e prever pontos de conexão acessíveis para ligação ao [BEP](/bep-barramento-equipotencializacao).

**Atenção normativa:** a NBR 5419:2026 proíbe a transição aço galvanizado no concreto → aço galvanizado no solo (par galvânico destrutivo). A transição deve ser feita com cobre ou aço inoxidável.

### Estratégia 5 — Aumento da profundidade e hastes especiais

A resistividade do solo frequentemente diminui com a profundidade, pois as camadas mais profundas tendem a ter maior umidade e teor mineral. A [medição de resistividade por Wenner](/resistividade-solo-metodo-wenner) com espaçamentos crescentes revela essa estratificação.

Quando a curva ρ × a indica camada profunda com resistividade significativamente menor:

- **Hastes extensíveis (emendáveis):** permitem cravação além de 3 m, atingindo camadas de menor resistividade. Hastes copperweld com rosca ou luva de emenda podem alcançar 6, 9 ou até 12 m.

- **Perfuração mecanizada:** em solo duro, a perfuração com martelete ou perfuratriz seguida de cravação e preenchimento com gel condutor é mais eficiente que múltiplas hastes rasas.

**Cuidado:** se a camada profunda é **mais** resistiva (caso de rocha sob argila), aumentar a profundidade da haste piora o resultado. A análise da curva de estratificação é obrigatória antes de decidir pela cravação profunda.

### Comparativo de eficiência das estratégias

EstratégiaRedução típica de RCusto relativoQuando usarHastes em paralelo42–65% (2 a 4 hastes)BaixoSolo moderado, espaço disponívelEletrodo horizontal30–60%MédioRocha superficial, lençol freático altoTratamento químico50–80%Médio-alto (R$ 1.500–6.000)Solo de alta resistividade (>500 Ω·m)Ferragem de fundação80–95% (quando disponível)Nenhum (existente)Edificações com fundação profundaHastes profundas/emendáveis40–70%MédioEstratificação favorável (ρ diminui com profundidade)
A combinação de estratégias é o cenário real da maioria dos projetos: ferragem de fundação como eletrodo principal + anel de aterramento (NBR 5419:2026) + hastes nos pontos de descida do SPDA + tratamento localizado nos pontos de maior exigência.

### O que não funciona

Práticas que persistem no mercado sem fundamentação técnica:

- **Jogar sal grosso no furo da haste:** redução temporária (semanas), seguida de corrosão acelerada e aumento da resistência
- **Usar carvão vegetal como condutor:** condutividade insuficiente, deterioração rápida
- **Cravar mais hastes sem respeitar espaçamento:** hastes a 50 cm uma da outra têm rendimento marginal — quase como uma haste única
- **Molhar o solo antes da medição para "dar laudo":** fraude técnica — a medição deve representar a condição mais desfavorável (período seco)

### Quando medir novamente após tratamento

Após qualquer intervenção para redução de R, a nova medição deve ser feita:

- Após estabilização do tratamento (mínimo 7 dias para bentonita, 30 dias para gel condutor)
- Preferencialmente no período seco (pior caso)
- Com o mesmo método e equipamento da medição original ([NBR 15749](/haste-aterramento-tipos-instalacao-medicao))

A periodicidade de reavaliação segue o padrão normativo: anual para edifícios e indústrias, trienal para demais estruturas.

### Conclusão técnica

Reduzir a resistência de aterramento exige diagnóstico da causa (resistividade do solo, geometria inadequada, conexões degradadas) antes da intervenção. A sequência racional é: verificar a ferragem de fundação como eletrodo natural, dimensionar hastes em paralelo com espaçamento correto (d ≥ L), considerar tratamento químico quando ρ > 500 Ω·m, e validar o resultado por medição no período seco. Adicionar hastes sem critério técnico é desperdício — quatro hastes corretamente posicionadas superam dez hastes amontoadas.

### Links relacionados

- → S5: Haste de Aterramento (`/haste-aterramento-tipos-instalacao-medicao`)
- → S9: Resistividade do Solo e Wenner (`/resistividade-solo-metodo-wenner`)
- → S11: Aterramento em Solo Rochoso (`/aterramento-solo-rochoso-solucoes`)
- → PILAR: Guia Completo de Aterramento (`/aterramento-eletrico-guia-completo`)
- → S12: Custos de Aterramento (`/custo-sistema-aterramento`)
- → S7: BEP (`/bep-barramento-equipotencializacao`)

Resistência de aterramento acima do necessário? A equipe AEOMaps faz o diagnóstico com base na resistividade real do solo e indica a estratégia de redução mais eficiente — sem sobredimensionamento.

**[Fale com um especialista pelo WhatsApp →](https://wa.me/5511925222281?text=Olá!%20Vim%20pelo%20artigo%20sobre%20redução%20de%20resistência%20de%20aterramento%20e%20preciso%20de%20orientação%20técnica.)**