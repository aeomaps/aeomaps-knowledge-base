---
title: "BEP — Barramento de Equipotencialização Principal: Função, Dimensionamento e Instalação"
slug: bep-barramento-equipotencializacao
date: 2026-06-07 09:00:00
categories: Aterramento
tags: aterramento, barramento, BEP, cobre, equipotencialização, NBR 5410, PE, SPDA
source: aeomaps.com.br/bep-barramento-equipotencializacao/
---

### O que é o BEP e por que existe

O BEP — Barramento de Equipotencialização Principal — é o ponto central onde todos os condutores de proteção, aterramento e equipotencialização se encontram. Sua função é garantir que todas as massas metálicas e elementos condutores estranhos à instalação elétrica estejam no mesmo potencial elétrico (equipotencial), eliminando diferenças de tensão que poderiam causar choque.

O termo BEP substituiu a designação anterior TAP (Terminal de Aterramento Principal) a partir da atualização da NBR 5410 em 2004, alinhando a terminologia brasileira à IEC. Na prática, muitos profissionais e fabricantes ainda utilizam TAP — mas a nomenclatura normativa atual é BEP.

O conceito fundamental é: toda corrente de falta deve encontrar um caminho de baixa impedância de volta à fonte. O BEP é o nó central desse caminho. Sem ele, partes metálicas da edificação podem ficar em potenciais diferentes durante uma falta — e a diferença de potencial entre duas massas acessíveis simultaneamente é o que causa [choque elétrico](/tensao-passo-toque-protecao-pessoas).

### Especificação física do BEP

A NBR 5410 e a prática de engenharia definem:

**Material:** barra de cobre eletrolítico nu (sem revestimento isolante), para permitir inspeção visual das conexões.

**Dimensões mínimas recomendadas:** 50 mm × 3 mm × 500 mm (largura × espessura × comprimento). Em instalações maiores, o comprimento é ajustado ao número de condutores que serão conectados — cada ponto de conexão precisa de espaço para terminal aparafusado.

**Fixação:** montada em isoladores sobre base não combustível, em local acessível para inspeção e manutenção. Não deve ser embutida em parede sem acesso — a verificação periódica das conexões é obrigatória.

**Furação:** furos para parafusos de conexão, tipicamente M6 a M10, com espaçamento que permita aperto com torquímetro sem interferência entre terminais adjacentes.

### Os 9 elementos da equipotencialização principal

A NBR 5410 (seção 6.4.2) define que ao BEP devem ser conectados:

#ElementoCondutor mínimo1Condutor de aterramento (do eletrodo ao BEP)Conforme tabela NBR 54102Condutor de proteção principal (PE geral)Conforme [dimensionamento PE](/dimensionamento-condutor-protecao-pe)3Condutores de equipotencialização (tubulações metálicas)6 mm² Cu4Tubulação de água fria6 mm² Cu5Tubulação de água quente / aquecimento6 mm² Cu6Tubulação de gás6 mm² Cu7Estrutura metálica da edificação6 mm² Cu8Armaduras de concreto armado (quando acessíveis)6 mm² Cu9Blindagem de cabos de telecomunicações6 mm² Cu
Nem todos os elementos estão presentes em toda edificação. Em uma residência sem gás canalizado e sem estrutura metálica aparente, os itens 6 e 7 não se aplicam. Mas a análise deve ser feita — e os elementos presentes devem ser conectados.

**Importante:** o condutor de equipotencialização deve ter seção mínima de 6 mm² em cobre. Não se aplica a tabela fase→PE aqui — o critério é diferente.

### Posição na instalação

O BEP deve estar localizado na **entrada da instalação** — tipicamente no quadro de medição ou no quadro de distribuição principal. É nesse ponto que:

- O PEN da concessionária (esquema TN-C-S) é dividido em PE + N
- O condutor de aterramento (vindo do eletrodo) chega ao barramento
- Os condutores de equipotencialização das tubulações metálicas convergem
- O condutor de descida do [SPDA](/aterramento-eletrico-guia-completo) (quando existente) é conectado

Em edificações com múltiplas entradas de energia ou com subestação própria, pode haver mais de um BEP — cada um na respectiva entrada. A interligação entre BEPs deve garantir equipotencialidade entre eles.

### Equipotencialização suplementar

Além da equipotencialização principal (BEP), a NBR 5410 prevê a **equipotencialização suplementar** em locais com risco aumentado:

**Banheiros (volumes 0, 1 e 2):** todas as massas e elementos condutores estranhos acessíveis nos volumes do chuveiro/banheira devem ser interligados por condutor de equipotencialização suplementar.

**Áreas com piscinas:** equipotencialização de bordas metálicas, escadas, drenos e partes metálicas acessíveis.

**Ambientes médicos:** equipotencialização suplementar de todas as massas ao alcance do paciente, com resistência máxima de 0,2 Ω entre qualquer par de massas.

O condutor de equipotencialização suplementar deve ter seção não inferior à do menor PE conectado às massas em questão, com mínimo de 2,5 mm² (se com proteção mecânica) ou 4 mm² (se sem proteção).

### BEP e NBR 5419:2026 (SPDA)

A integração entre o sistema de aterramento da instalação e o SPDA (Sistema de Proteção contra Descargas Atmosféricas) passa pelo BEP:

- O anel de aterramento exigido pela NBR 5419:2026 deve ser conectado ao BEP
- Os condutores de descida do SPDA devem ser interligados ao anel e ao BEP
- DPS (Dispositivos de Proteção contra Surtos) são instalados no quadro de entrada, com referência ao BEP

A equipotencialização no BEP impede que descargas atmosféricas criem diferenças de potencial entre o SPDA e a instalação interna. Sem essa integração, um raio pode causar centelhamento entre o sistema de proteção e instalações internas — danificando equipamentos e gerando risco de incêndio.

### BEP em sistemas fotovoltaicos

Em instalações [fotovoltaicas](/aterramento-sistema-fotovoltaico-nbr16690), o BEP recebe também:

- Condutor de equipotencialização das estruturas metálicas dos módulos (lado CC)
- Aterramento funcional do ponto médio ou negativo do string (quando aplicável)
- Condutor de proteção do inversor (lado CA)

A equipotencialização dos lados CC e CA no mesmo BEP é o princípio fundamental — as massas metálicas do array fotovoltaico devem estar no mesmo potencial que as massas da instalação convencional.

### Erros frequentes na instalação do BEP

**1. BEP inacessível**

Embutir o BEP dentro de parede sem portinhola de inspeção é erro grave. As conexões aparafusadas precisam de verificação periódica — torque, oxidação, aquecimento.

**2. Conexões por enrolamento de fio**

Cada condutor deve ter terminal adequado (terminal de pressão, olhal ou compressão), apertado com torque conforme especificação do fabricante. Fio enrolado no parafuso não é conexão normativa.

**3. BEP pintado ou envernizado**

A barra de cobre deve ser nua. Pintura ou verniz isolam as superfícies de contato e aumentam a resistência das conexões — exatamente o oposto da função do BEP.

**4. Não conectar tubulações metálicas**

A tubulação de água que atravessa a edificação e não está conectada ao BEP pode ficar em potencial diferente das massas elétricas durante uma falta. Pessoa tocando simultaneamente torneira e carcaça de equipamento pode receber choque.

**5. Confundir BEP com barra de neutro**

O BEP é exclusivo para proteção e equipotencialização. A barra de neutro é para distribuição do condutor neutro (N). No esquema TN-C-S, o PEN chega e é dividido: neutro vai para a barra de neutro, PE vai para o BEP. São barramentos fisicamente separados.

**6. Usar a mesma barra para BEP e neutro em TN-S**

No esquema TN-S, PE e N são condutores separados desde o transformador. Conectá-los em uma mesma barra dentro do quadro transforma o TN-S em TN-C a partir daquele ponto — violação normativa que cria corrente de neutro no PE.

### Verificação e manutenção

A verificação do BEP inclui:

- **Inspeção visual:** oxidação, aquecimento (escurecimento), folga nos parafusos, integridade dos terminais
- **Medição de continuidade:** resistência entre o BEP e cada massa conectada deve ser 
BEP ausente, subdimensionado ou mal posicionado? A equipe AEOMaps projeta a equipotencialização completa — desde o barramento até a integração com SPDA e sistemas fotovoltaicos.

**[Fale com um especialista pelo WhatsApp →](https://wa.me/5511925222281?text=Olá!%20Vim%20pelo%20artigo%20sobre%20BEP%20e%20preciso%20de%20orientação%20técnica.)**