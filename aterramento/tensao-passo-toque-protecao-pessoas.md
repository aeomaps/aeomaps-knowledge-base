---
title: "Tensão de Passo, Tensão de Toque e Proteção de Pessoas em Sistemas de Aterramento"
slug: tensao-passo-toque-protecao-pessoas
date: 2026-06-07 12:55:16
categories: Aterramento
tags: aterramento, choque elétrico, efeitos fisiológicos, NBR 5419, proteção, tensão de contato, tensão de passo, tensão de toque
source: aeomaps.com.br/tensao-passo-toque-protecao-pessoas/
---

### O que acontece quando uma corrente de falta atinge o solo

Quando uma corrente de falta — por defeito de isolamento ou descarga atmosférica — é drenada para o solo através do [eletrodo de aterramento](/haste-aterramento-tipos-instalacao-medicao), ela se distribui de forma não uniforme pelo terreno. O potencial elétrico do solo é máximo no ponto de injeção (eletrodo) e diminui com a distância.

Essa distribuição gera gradientes de potencial que podem expor pessoas a tensões perigosas, mesmo sem contato direto com partes energizadas. É esse gradiente que define os conceitos de tensão de passo e tensão de toque.

### Distribuição de potencial no solo

A corrente que entra no solo pelo eletrodo se dispersa radialmente. A resistência do solo não é concentrada — ela se distribui ao longo do volume de terra ao redor do eletrodo. No entanto, essa distribuição é fortemente concentrada nos primeiros metros.

Dado quantitativo fundamental: cerca de 50% da resistência total do eletrodo se concentra nos primeiros 15 cm ao redor da haste. Nos primeiros 3 metros de raio, aproximadamente 90% da queda de potencial já ocorreu.

Se uma haste de aterramento drena uma corrente de falta, e o potencial na superfície do solo junto à haste é de 12.500 V, a queda de potencial é extremamente abrupta. A diferença de potencial entre dois pontos separados por apenas um passo (≈ 1 metro) pode ser de centenas ou milhares de volts.

### Tensão de passo

Tensão de passo é a diferença de potencial entre dois pontos do solo separados pela distância de um passo humano (convencionalmente 1 metro), medida na direção radial a partir do eletrodo de aterramento.

Uma pessoa caminhando próxima ao ponto de injeção de corrente no solo fica sujeita a essa diferença de potencial entre seus pés. A corrente resultante percorre o caminho pé-pé, atravessando as pernas.

Características da tensão de passo:

- Máxima nas proximidades imediatas do eletrodo
- Diminui rapidamente com a distância
- Depende da resistividade do solo, da magnitude da corrente de falta e da geometria do eletrodo
- O caminho da corrente (pé-pé) passa pela região pélvica, não pelo tórax

A tensão de passo é particularmente perigosa durante descargas atmosféricas em campo aberto e em subestações de alta tensão durante faltas à terra.

### Tensão de toque

Tensão de toque é a diferença de potencial entre uma massa metálica (equipamento, estrutura, cerca) acessível ao toque e o ponto do solo onde a pessoa está de pé.

Quando um equipamento com falha de isolamento transfere potencial para sua carcaça, a pessoa que toca essa carcaça fica sujeita à diferença entre o potencial da massa e o potencial do solo sob seus pés. A corrente resultante percorre o caminho mão-pé, atravessando o tórax.

Essa é a condição mais perigosa: corrente atravessando a região torácica atinge o coração, com risco direto de fibrilação ventricular.

### Tensão de contato

Tensão de contato é o termo mais abrangente: a tensão que efetivamente aparece entre duas partes do corpo de uma pessoa ao tocar simultaneamente dois pontos com potenciais diferentes. Pode ser uma combinação de tensão de toque (mão-pé) ou outras configurações (mão-mão, por exemplo).

A NBR 5410 define tensão limite de contato (UL):

CondiçãoULCondições normais (locais secos)50 VCondições especiais (locais úmidos, canteiros)25 V
Esses valores são os limites acima dos quais a proteção contra contatos indiretos deve atuar automaticamente.

### Efeitos fisiológicos da corrente elétrica no corpo humano

A gravidade do choque depende da magnitude da corrente que atravessa o corpo, do caminho percorrido e do tempo de exposição. Os efeitos são progressivos:

Corrente (mA)Efeito fisiológico~1Percepção (formigamento)~5Eletrização (movimentos involuntários)10Tetanização (agarramento — a pessoa não consegue soltar)25Parada respiratória~30Asfixia (corrente pelo tórax)60–75Fibrilação ventricular (risco de morte)
O limiar de fibrilação ventricular — 60 a 75 mA — é atingido com tensões relativamente baixas quando a resistência do corpo é reduzida por umidade, suor, ferimentos ou contato com grandes superfícies metálicas.

O caminho mão-pé (tensão de toque) é mais perigoso que pé-pé (tensão de passo) porque a corrente atravessa a região cardíaca. Por isso, a tensão de toque recebe mais atenção no dimensionamento de proteção.

### Por que o aterramento reduz (mas não elimina) o risco

O sistema de aterramento cumpre duas funções para a proteção de pessoas:

**Limitar a tensão de contato:** ao conectar todas as massas ao sistema de aterramento (equipotencialização), a diferença de potencial entre partes acessíveis é minimizada. Quanto menor a resistência do eletrodo, menor a elevação de potencial da massa em relação ao solo remoto durante uma falta.

**Viabilizar a atuação dos dispositivos de proteção:** a corrente de falta, ao circular pelo sistema de aterramento, deve ser suficiente para sensibilizar o dispositivo de proteção (DR, disjuntor) no tempo exigido pela norma.

Porém, o aterramento sozinho não garante segurança. A proteção depende do conjunto: eletrodo + equipotencialização + dispositivo de proteção + dimensionamento correto.

### Medidas práticas de proteção contra tensão de passo e toque

**Equipotencialização:** conectar todas as massas, tubulações metálicas, estruturas, ferragens e eletrodos ao [BEP (Barramento de Equipotencialização Principal)](/bep-barramento-equipotencializacao). A equipotencialização reduz a diferença de potencial entre pontos acessíveis simultaneamente.

**Malha de aterramento com gradiente controlado:** em subestações e instalações de grande porte, a malha de cabos enterrada equaliza o potencial da superfície do solo, reduzindo o gradiente de tensão de passo. O dimensionamento segue critérios do IEEE Std 80.

**Camada superficial de alta resistividade:** aplicação de brita ou material isolante sobre o solo na área de operação. A camada de brita (tipicamente 3.000 Ω·m) aumenta a resistência de contato entre os pés e o solo, reduzindo a corrente que atravessa o corpo.

**Dispositivos de proteção adequados:** DR com sensibilidade compatível com a tensão limite de contato. Em locais úmidos e [canteiros de obras](/aterramento-canteiro-obras-nr10-nr18), a norma reduz UL para 25 V, exigindo DR de maior sensibilidade ou resistência de aterramento mais baixa.

**Restrição de acesso:** em subestações e áreas com gradientes de potencial significativos, cercas e barreiras evitam o acesso de pessoas não qualificadas durante faltas.

### Caso prático: descarga atmosférica em haste isolada

Uma descarga atmosférica injeta uma corrente de pico da ordem de 30 kA no solo por uma haste de aterramento. Se a resistência do eletrodo é 20 Ω, o potencial da haste em relação ao solo remoto atinge 600 kV.

A tensão de passo a 1 metro da haste pode ultrapassar 100 kV. Uma pessoa caminhando nessa região sofre um choque pé-pé potencialmente fatal, mesmo sem tocar em nada.

Isso demonstra por que o SPDA exige eletrodo em anel (NBR 5419:2026), não apenas hastes isoladas: o anel distribui a corrente em um perímetro, reduzindo o gradiente de potencial na superfície.

### Conclusão técnica

Tensão de passo e tensão de toque são consequências diretas da distribuição de potencial no solo durante uma falta. A gravidade depende da magnitude da corrente, da geometria do eletrodo, da resistividade do solo e do caminho percorrido pela corrente no corpo.

A proteção efetiva exige: equipotencialização completa, dispositivos de proteção corretamente dimensionados, geometria do eletrodo que controle o gradiente de potencial e, em subestações, camada superficial de alta resistividade.

### Links relacionados

- [Guia Completo de Aterramento](/aterramento-eletrico-guia-completo) — visão geral do sistema de proteção
- [Haste de Aterramento](/haste-aterramento-tipos-instalacao-medicao) — eletrodo e distribuição de potencial
- [Dimensionamento do Condutor PE](/dimensionamento-condutor-protecao-pe) — proteção contra contatos indiretos
- [O Mito dos 10Ω](/mito-10-ohms-resistencia-aterramento) — valor de resistência e proteção de pessoas

Projeto de aterramento com análise de tensão de passo e toque? A equipe AEOMaps dimensiona o sistema com base na corrente de falta, resistividade do solo e geometria dos eletrodos.

**[Fale com um especialista pelo WhatsApp →](https://wa.me/5511925222281?text=Olá!%20Vim%20pelo%20artigo%20sobre%20tensão%20de%20passo%20e%20toque%20e%20preciso%20de%20orientação%20técnica.)**