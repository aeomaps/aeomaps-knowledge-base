---
title: "Aterramento para Equipamentos Eletrônicos: Ponto Único, Malha de Terra de Referência e Blindagem"
slug: aterramento-equipamentos-eletronicos-mtr
date: 2026-06-07 12:58:30
categories: Aterramento
tags: blindagem, CLP, DPS, eletrônicos, EMI, inversor, modo comum, MTR, ponto único, ruído
source: aeomaps.com.br/aterramento-equipamentos-eletronicos-mtr/
---

### O problema: aterramento de força não serve para eletrônica

Nos anos 1970 e 1980, a indústria brasileira começou a substituir painéis eletromecânicos por CLPs e equipamentos com circuitos integrados. A solução de aterramento da época era ligar tudo à mesma malha de força — a mesma usada por motores, partidas de compressores e máquinas de solda. O resultado foi desastroso: travamentos, queima inexplicável de placas, perda de comunicação serial e falhas intermitentes que desafiavam qualquer lógica de diagnóstico.

O motivo é simples: equipamentos de força e equipamentos eletrônicos têm exigências de aterramento opostas. Para a força, o aterramento é um caminho de baixa impedância para correntes de falta (dezenas ou centenas de ampères, 60 Hz). Para a eletrônica, o aterramento é uma referência de potencial estável — qualquer oscilação de milivolt na referência pode corromper dados, disparar surtos de modo comum ou danificar componentes sensíveis a ESD.

Conectar ambos à mesma barra sem isolamento galvânico significa que a corrente de partida de um motor de 50 cv injeta ruído diretamente no plano de referência do CLP. É a causa número um de falhas crônicas em automação industrial.

### Sintomas de aterramento deficiente em equipamentos eletrônicos

Antes de detalhar as soluções, vale reconhecer os sintomas — porque muitos técnicos convivem com eles sem identificar a causa:

SintomaEquipamento típicoMecanismoQuebra intermitente de comunicação RS-232/RS-485CLPs, supervisórios, balançasDiferença de potencial entre terras das duas pontasInterferência eletromagnética (EMI) em instrumentaçãoMedidores de vazão, células de cargaCorrente de modo comum no cabo de sinalAquecimento anormal de inversores de frequênciaDrives ACCorrente de fuga pelo filtro EMC circulando por caminho inadequadoTravamentos aleatórios de softwareIHMs, computadores industriaisRuído no barramento de dados via plano de terraQueima inexplicável de CIs e portas de comunicaçãoPlacas eletrônicas, interfacesSobretensão transitória sem caminho de dissipaçãoLeitura errática de sensores analógicosTermopares, transmissores 4-20 mALoop de terra entre fonte e receptorReset espontâneo de equipamentosControladores, relés inteligentesPerturbação no rail de alimentação via acoplamento condutivo
Se a planta apresenta dois ou mais desses sintomas simultaneamente, a probabilidade de o problema estar no aterramento — e não nos equipamentos — é elevada.

### Conceitos fundamentais: modo comum e modo diferencial

Para entender as soluções, é necessário distinguir dois tipos de ruído:

**Ruído de modo diferencial:** aparece entre os condutores de sinal (por exemplo, entre os fios de um par RS-485). Causa: acoplamento capacitivo ou indutivo de cabos de força próximos. Solução principal: blindagem e separação física.

**Ruído de modo comum:** aparece entre os condutores de sinal e a referência de terra. Causa: diferença de potencial entre os pontos de aterramento dos equipamentos interligados. É o ruído mais destrutivo em instalações industriais, porque atinge todos os condutores simultaneamente e não é eliminado por filtros diferenciais comuns.

O ruído de modo comum é o inimigo direto de qualquer rede de comunicação industrial. Se dois CLPs estão a 200 metros de distância e cada um está aterrado em um ponto diferente da malha de força, a diferença de potencial entre os dois terras pode chegar a dezenas de volts durante a partida de uma carga pesada. Essa tensão aparece integralmente no cabo de comunicação — e portas RS-232 suportam, no máximo, ±15 V.

### Solução 1: ponto único de referência (estrela)

A primeira estratégia é o aterramento em ponto único, também chamado de aterramento em estrela. O princípio: todos os equipamentos eletrônicos de um mesmo sistema convergem para um único ponto de conexão ao aterramento — e nenhum deles se conecta diretamente à malha de força em outro ponto.

**Regras do ponto único:**

- Definir um barramento de referência exclusivo para eletrônica, separado do [BEP](/bep-barramento-equipotencializacao) da instalação de força
- Conectar o barramento de referência ao BEP em **um único ponto** — por condutor dedicado, curto e de seção generosa (mínimo 16 mm² Cu)
- Cada equipamento eletrônico se liga ao barramento de referência por condutor individual (nunca em cascata — "daisy chain")
- O barramento de referência fica próximo ao centro geométrico dos equipamentos, não na extremidade

O ponto único funciona bem para frequências baixas (até ~1 MHz). Para frequências mais altas — presentes em inversores de frequência com chaveamento PWM, fontes chaveadas e comunicação digital de alta velocidade — o comprimento dos condutores de referência introduz indutância suficiente para comprometer a equipotencialidade. Nesse caso, a M.T.R. é a solução.

### Solução 2: Malha de Terra de Referência (M.T.R.)

A Malha de Terra de Referência — M.T.R. — é um plano condutor instalado sob os equipamentos eletrônicos para criar uma referência de potencial equipotencial em alta frequência. Diferente do ponto único (que funciona por topologia), a M.T.R. funciona por geometria: a malha tem dimensões muito menores que o comprimento de onda dos sinais, garantindo que não há diferença de potencial significativa entre quaisquer dois pontos.

**Critério de dimensionamento:**

A abertura da malha (distância entre condutores paralelos) deve ser menor que λ/20, onde λ é o comprimento de onda da frequência mais alta de interesse.

Frequênciaλ (m)Abertura máxima (λ/20)1 MHz30015 m10 MHz301,5 m30 MHz100,5 m (50 cm)60 MHz50,25 m (25 cm)100 MHz30,15 m (15 cm)
Na prática industrial, a M.T.R. mais comum usa malha de 30 cm × 30 cm — adequada para frequências de até 50 MHz, cobrindo a maioria das aplicações de automação industrial e inversores de frequência. Para data centers com comunicação Ethernet de alta velocidade (100 MHz+), a malha deve ser de 15 cm ou menor.

**Construção da M.T.R.:**

- Material: fita ou barra de cobre nu, ou chapa de cobre perfurada
- Instalada sob o piso falso ou diretamente sob os gabinetes eletrônicos
- Todos os cruzamentos soldados ou aparafusados com contato metálico direto (não usar cabos isolados)
- Cada gabinete ou rack conectado à M.T.R. por múltiplos pontos — quanto mais, melhor
- A M.T.R. é conectada ao [sistema de aterramento geral](/aterramento-eletrico-guia-completo) em múltiplos pontos (diferente do ponto único)

**Diferença fundamental:** o ponto único usa topologia em estrela com um condutor por equipamento; a M.T.R. usa topologia em malha com múltiplas conexões. São complementares: o ponto único é adequado para sinais de baixa frequência, a M.T.R. para alta frequência. Em instalações complexas (data centers, salas de controle de processo), ambos coexistem.

### Solução 3: blindagem de cabos

A blindagem é a primeira linha de defesa contra acoplamento eletromagnético em cabos de sinal e comunicação. Mas blindagem mal aterrada não protege — pode até piorar o problema.

**Regras de aterramento da blindagem:**

Tipo de sinalFrequência predominanteAterramento da blindagemAnalógico baixa frequência (4-20 mA, termopar)Uma extremidade apenas (lado da fonte ou receptor, nunca ambos)Digital baixa velocidade (RS-232, RS-485)Uma extremidade (lado do mestre/controlador)Digital alta velocidade (Ethernet, Profinet)> 1 MHzAmbas as extremidadesInstrumentação com blindagem duplaMistoBlindagem interna em uma ponta, externa em ambas
**Por que uma extremidade para baixa frequência?** Se a blindagem é aterrada nas duas pontas e existe diferença de potencial entre os dois pontos de aterramento (o que é praticamente garantido em plantas industriais), uma corrente circula pela blindagem. Essa corrente induz ruído nos condutores internos — exatamente o oposto do que se deseja.

**Por que ambas as extremidades para alta frequência?** Acima de ~1 MHz, a impedância indutiva da blindagem aterrada em uma ponta é alta o suficiente para que a blindagem perca eficácia. O aterramento em ambas as pontas cria um caminho de baixa impedância em alta frequência, que é o que importa.

### Solução 4: isolamento galvânico

Quando a diferença de potencial entre dois pontos de aterramento é estrutural (plantas extensas, edifícios diferentes, subestações separadas), o isolamento galvânico elimina o problema na raiz: rompe o caminho elétrico entre os dois sistemas.

**Técnicas de isolamento galvânico:**

- **Transformador de isolamento:** na entrada da alimentação dos equipamentos eletrônicos. Cria um novo sistema TN-S local, com referência de terra independente. O secundário do transformador é aterrado no barramento de referência da eletrônica — não na malha de força
- **Fibra óptica:** para comunicação entre equipamentos em potenciais de terra diferentes. Elimina 100% do acoplamento condutivo e eletromagnético. Conversores de mídia em cada ponta, cada um aterrado no seu sistema local
- **Conversores isolados:** para sinais analógicos (isoladores galvânicos 4-20 mA, optoacopladores). Cada isolador rompe a continuidade do terra de sinal entre fonte e receptor
- **Relés de interface:** para sinais digitais discretos entre sistemas com terras diferentes. A bobina está em um sistema, o contato no outro — sem conexão galvânica

### Solução 5: DPS e proteção contra surtos

Mesmo com M.T.R., ponto único e blindagem, os equipamentos eletrônicos precisam de proteção contra surtos transitórios — especialmente descargas atmosféricas indiretas e chaveamento de cargas indutivas.

A filosofia é a proteção coordenada em cascata:

- **DPS Classe I (tipo 1):** no quadro geral, próximo ao BEP. Suporta correntes de descarga de 12,5 a 50 kA (onda 10/350 μs). Limita surtos de origem atmosférica
- **DPS Classe II (tipo 2):** nos quadros de distribuição secundários. Limita surtos residuais do Classe I e surtos de chaveamento
- **DPS Classe III (tipo 3):** na entrada dos equipamentos eletrônicos sensíveis. Tensão de proteção (Up) ≤ 1,5 kV. Instalado o mais próximo possível do equipamento

**Regra crítica:** o condutor de conexão do DPS ao barramento de terra deve ser o mais curto possível — cada metro de condutor adiciona ~1 kV à tensão de proteção efetiva durante um surto. O ideal é que o DPS esteja a menos de 50 cm do barramento.

Para linhas de comunicação (RS-485, Ethernet), existem DPS específicos que limitam a sobretensão entre os condutores de sinal e entre sinal e terra. Sem essa proteção, uma descarga atmosférica a 2 km de distância pode queimar portas de comunicação por surto induzido.

### Projeto integrado: quando combinar as soluções

Na prática, nenhuma das soluções acima funciona isoladamente em instalações complexas. A estratégia depende do porte e da criticidade da aplicação:

AplicaçãoPonto únicoM.T.R.BlindagemIsolamentoDPSPequena automação (1-2 CLPs)✅—✅—✅ (Classe II+III)Sala de controle industrial✅✅ (30 cm)✅✅ (transformador)✅ (I+II+III)Data center—✅ (15 cm)✅✅ (fibra)✅ (I+II+III)Instrumentação de campo✅—✅✅ (isoladores)✅ (II+III)Telecomunicações (torre)—✅✅✅ (fibra + transformador)✅ (I+II+III)
A M.T.R. complementa, mas não substitui, o aterramento convencional da instalação. O [sistema de aterramento de proteção](/aterramento-eletrico-guia-completo) (eletrodo, PE, BEP) permanece obrigatório conforme NBR 5410. A M.T.R. é uma camada adicional, específica para a referência de potencial em alta frequência.

### Erros frequentes no aterramento de eletrônicos

- **Usar o condutor neutro como referência de terra:** o neutro carrega corrente de retorno — sua tensão varia com a carga. Nunca usar N como referência para circuitos eletrônicos. A [diferença entre terra e neutro](/diferenca-terra-neutro-massa) é fundamental
- **Aterramento em cascata (daisy chain):** conectar equipamentos em série no condutor de terra. Cada equipamento adiciona impedância ao caminho do próximo — os últimos da cadeia ficam com referência instável
- **Blindagem aterrada nas duas pontas para sinais analógicos de baixa frequência:** cria loop de terra, injeta ruído em vez de eliminá-lo
- **Separar completamente o terra da eletrônica do terra da força:** terras separados sem conexão criam diferença de potencial perigosa entre as massas. O terra da eletrônica deve ser separado operacionalmente, mas conectado eletricamente ao BEP em ponto único
- **DPS com condutor de terra longo:** cada metro de condutor adiciona ~1 μH de indutância, elevando a tensão de proteção em até 1 kV por metro durante um surto. O DPS perde a função

### Checklist para diagnóstico de campo

Ao investigar problemas de aterramento em equipamentos eletrônicos:

- Medir a [resistência do sistema de aterramento](/haste-aterramento-tipos-instalacao-medicao) — não é suficiente que seja baixa; precisa estar no valor calculado conforme o [esquema de aterramento (TT, TN ou IT)](/sistemas-tt-tn-it-diferencas)
- Medir a tensão entre o terra do equipamento problemático e o terra do equipamento de referência (osciloscópio, com sonda de corrente de modo comum)
- Verificar se existe mais de um ponto de conexão ao sistema de aterramento (loops)
- Verificar se a blindagem dos cabos de sinal está aterrada corretamente (uma ou duas pontas, conforme a frequência)
- Verificar se existem motores, inversores ou máquinas de solda compartilhando o mesmo barramento de terra que os eletrônicos
- Verificar se o DPS está instalado e se o condutor de conexão é curto (
Problemas de ruído, queima de CIs ou falhas intermitentes em equipamentos eletrônicos? A equipe AEOMaps analisa o sistema de aterramento e indica a solução técnica adequada — ponto único, M.T.R., blindagem ou isolamento galvânico.

**[Fale com um especialista pelo WhatsApp →](https://wa.me/5511925222281?text=Olá!%20Preciso%20de%20ajuda%20com%20aterramento%20para%20equipamentos%20eletrônicos.)**