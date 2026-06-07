---
title: "Aterramento de Sistemas Fotovoltaicos: NBR 16690, Equipotencialização CC/CA e Compatibilidade com SPDA"
slug: aterramento-sistema-fotovoltaico-nbr16690
date: 2026-06-07 12:57:19
categories: Aterramento
tags: aterramento, DPS, equipotencialização, fotovoltaico, inversor, NBR 16690, solar, SPDA
source: aeomaps.com.br/aterramento-sistema-fotovoltaico-nbr16690/
---

### Por que o aterramento fotovoltaico é obrigatório

A instalação de um sistema fotovoltaico (FV) em uma edificação é classificada como reforma elétrica — e toda reforma obriga a adequação do sistema de aterramento à norma vigente. Não importa se a edificação é antiga e não tinha aterramento: a partir da instalação do sistema FV, o aterramento passa a ser obrigatório.

As normas aplicáveis:

- **NBR 16690:2019** — Instalações elétricas de arranjos fotovoltaicos (cancelada e em revisão; princípios técnicos permanecem referência)
- **NBR 5410:2004** — Instalações elétricas de baixa tensão (lado CA)
- **NBR 5419:2026** — Proteção contra descargas atmosféricas
- **NBR 17193:2025** — Detecção de arco em sistemas FV

O aterramento em sistemas FV tem dupla função: proteção contra choques (correntes de falta) e proteção contra sobretensões (descargas atmosféricas e surtos induzidos). Os módulos fotovoltaicos operam em tensões CC de 200 a 1.000 V — tensões que causam arcos sustentados e incêndios quando o aterramento é deficiente.

### Dois aterramentos distintos: proteção e funcional

Em sistemas fotovoltaicos, existem dois conceitos de aterramento que não devem ser confundidos:

**Aterramento de proteção:** conexão de todas as partes metálicas não energizadas (molduras dos módulos, estrutura de fixação, carcaça do inversor, eletrocalhas, quadros) ao sistema de aterramento por meio do [condutor de proteção PE](/dimensionamento-condutor-protecao-pe). Função: proteger contra choques em caso de falha de isolamento.

**Aterramento funcional:** conexão intencional de um ponto do circuito CC (tipicamente o negativo ou o ponto médio) à terra. Função: definir uma referência de potencial para o sistema CC, limitar sobretensões e permitir a atuação de dispositivos de proteção contra falta à terra.

Nem todo sistema FV tem aterramento funcional. Inversores sem transformador de isolamento (a maioria dos modelos atuais) frequentemente operam com sistema CC flutuante (sem aterramento funcional) — e nesse caso, a detecção de falta à terra é feita por monitoramento de isolamento integrado ao inversor.

### Equipotencialização CC e CA no mesmo BEP

O princípio fundamental do aterramento FV é: **todas as massas metálicas do lado CC (array) e do lado CA (instalação convencional) devem estar conectadas ao mesmo [BEP](/bep-barramento-equipotencializacao)**.

**Lado CC — o que conectar ao BEP:**

- Molduras metálicas dos módulos FV
- Estrutura de fixação (perfis de alumínio, trilhos)
- Eletrocalhas e eletrodutos metálicos do trecho CC
- Carcaça do inversor (lado CC)
- String box (quando metálica)

**Lado CA — o que já deve estar conectado ao BEP:**

- PE do quadro de distribuição CA
- Tubulações metálicas (água, gás)
- Estrutura metálica da edificação
- Armaduras de concreto armado

A interligação é feita por condutores de equipotencialização com seção mínima de 6 mm² Cu. As conexões na estrutura metálica do array devem ser por parafusos inoxidáveis com arruela serrilhada (para garantir contato através do anodizado do alumínio) ou por conector de aterramento específico para FV.

**Erro comum:** tratar o aterramento do array FV como sistema separado do aterramento da edificação. Dois aterramentos independentes criam diferença de potencial entre as massas CC e CA — exatamente o oposto da equipotencialização.

### Aterramento funcional — ponto único

Quando o sistema tem aterramento funcional (conexão do negativo ou ponto médio à terra), a conexão deve ser feita em **ponto único**, próximo ao inversor. Múltiplos pontos de aterramento funcional criam caminhos paralelos de corrente pelo solo, gerando:

- Correntes parasitas CC no solo
- Corrosão eletrolítica em tubulações metálicas enterradas
- Interferência em sistemas de comunicação
- Erro de leitura em dispositivos de proteção contra falta à terra

O ponto único de aterramento funcional geralmente coincide com o terminal de aterramento do inversor, que é conectado ao BEP por condutor dedicado.

### Compatibilidade com SPDA (NBR 5419)

Módulos fotovoltaicos instalados em telhados ficam expostos a descargas atmosféricas. A compatibilidade entre o sistema FV e o SPDA é regulada pela NBR 5419-3:

**Distância de segurança:** os módulos FV devem manter distância de segurança dos condutores de descida e captores do SPDA. A distância mínima é calculada pela fórmula da NBR 5419-3 e depende do nível de proteção, comprimento do condutor de descida e material do condutor.

**Quando a distância não pode ser mantida:** se os módulos estão muito próximos do SPDA (situação comum em telhados pequenos), a solução é a equipotencialização — conectar a estrutura metálica do array ao SPDA, garantindo que ambos estejam no mesmo potencial durante uma descarga.

**Anel de aterramento (NBR 5419:2026):** o anel obrigatório ao redor da edificação beneficia diretamente o sistema FV, pois cria uma malha equipotencial que distribui a corrente de descarga e reduz gradientes de potencial.

**DPS (Dispositivos de Proteção contra Surtos):** obrigatórios em ambos os lados:

- **Lado CC:** DPS tipo 2 (mínimo) no string box ou na entrada CC do inversor
- **Lado CA:** DPS tipo 2 no quadro de distribuição CA
- Se a edificação tem SPDA ou está em região de alta incidência de raios: DPS tipo 1 + tipo 2 (coordenados)

### Detecção de falta à terra no sistema FV

A detecção de falta à terra em sistemas FV tem particularidades:

**Inversores com transformador de isolamento:** o lado CC é galvanicamente isolado do CA. Uma falta à terra no lado CC é detectada pelo monitoramento de isolamento do inversor, que sinaliza alarme e pode desligar o sistema.

**Inversores sem transformador (transformerless):** o lado CC e CA não são galvanicamente isolados. Correntes de fuga capacitivas circulam naturalmente entre os módulos e a terra (através da capacitância parasita do módulo com a estrutura/telhado). Essas correntes aumentam com a área do array e com a umidade. O inversor deve monitorar essas correntes e distinguir entre fuga normal e falta real.

**AFCI (Arc Fault Circuit Interrupter):** a NBR 17193:2025 introduz requisitos de detecção de arco em série no lado CC. Arcos CC são autossustentados e causam incêndios. Inversores modernos incorporam detecção AFCI — um motivo adicional para que as conexões de aterramento estejam íntegras (arco em conector de aterramento solto pode ser interpretado como falta de arco no string).

### Particularidades de instalação

**Telhado metálico:** quando o sistema FV é instalado sobre telhado metálico (telha galvanizada, alumínio), a própria cobertura funciona como plano de equipotencialização. A estrutura de fixação em contato com o telhado metálico já está equipotencializada — mas a continuidade elétrica deve ser verificada (parafusos com arruela de contato, não apenas apoio mecânico).

**Laje de concreto:** a estrutura de fixação é ancorada na laje, sem contato elétrico natural com as armaduras internas. Os condutores de equipotencialização devem interligar explicitamente a estrutura do array ao sistema de aterramento.

**Solo (usinas de solo):** a estrutura metálica de fixação está em contato direto com o solo através das estacas. Cada mesa de módulos deve ser equipotencializada e conectada ao anel/malha de aterramento da usina. A resistividade do solo determina a configuração do [aterramento por Wenner](/resistividade-solo-metodo-wenner).

**Flutuante sobre água (floating solar):** aplicação de nicho crescente — aterramento por cabo subaquático conectado a eletrodo em terra firme. Projeto específico, fora do escopo das normas convencionais.

### Manutenção do aterramento FV

A manutenção do aterramento em sistemas FV inclui:

- **Verificação de continuidade:** medir resistência entre cada moldura de módulo e o BEP. Valores acima de 1 Ω indicam conexão degradada.
- **Inspeção visual:** oxidação nos conectores de aterramento, parafusos soltos, condutores danificados por radiação UV ou roedores
- **Medição de isolamento CC:** resistência de isolamento entre positivo/terra e negativo/terra, com megôhmetro a 500 V CC (mínimo 1 MΩ por regra geral; verificar especificação do inversor)
- **Teste de DPS:** verificação visual dos indicadores de estado dos DPS (janela verde/vermelha)
- **Periodicidade:** anual para sistemas residenciais; semestral para usinas comerciais e industriais

### Conclusão técnica

O aterramento de sistemas fotovoltaicos exige equipotencialização dos lados CC e CA no mesmo BEP, aterramento funcional em ponto único (quando aplicável), compatibilidade com SPDA (distância de segurança ou equipotencialização), DPS nos lados CC e CA, e monitoramento de falta à terra pelo inversor. A instalação de um sistema FV é reforma elétrica — obriga adequação do aterramento. Módulos operando a centenas de volts CC em telhados expostos a intempéries não admitem improvisação no aterramento.

### Links relacionados

- → S7: BEP (`/bep-barramento-equipotencializacao`)
- → S5: Haste de Aterramento (`/haste-aterramento-tipos-instalacao-medicao`)
- → S8: Condutor PE (`/dimensionamento-condutor-protecao-pe`)
- → S9: Resistividade e Wenner (`/resistividade-solo-metodo-wenner`)
- → PILAR: Guia Completo (`/aterramento-eletrico-guia-completo`)
- → S6: Tensão de Passo e Toque (`/tensao-passo-toque-protecao-pessoas`)

Instalando sistema fotovoltaico e precisa garantir aterramento e compatibilidade com SPDA? A equipe AEOMaps projeta a equipotencialização CC/CA e o sistema de proteção contra surtos.

**[Fale com um especialista pelo WhatsApp →](https://wa.me/5511925222281?text=Olá!%20Vim%20pelo%20artigo%20sobre%20aterramento%20fotovoltaico%20e%20preciso%20de%20orientação%20técnica.)**