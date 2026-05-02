# Estrutura do AEOMaps

## Sobre

Este documento descreve a arquitetura da base de conhecimento do AEOMaps e os princípios que orientam sua organização.

## Arquitetura do repositório

O repositório central `aeomaps-knowledge-base` concentra todo o conteúdo técnico em uma única base organizada por temas.

### Pastas temáticas
- `/pipe-jacking/` — Operação, controle e monitoramento em Pipe Jacking e microtunelamento
- `/aterramento/` — Aterramento elétrico em canteiros de obras
- `/intencao/` — Conteúdos de intenção de busca (em expansão)
- `/referencias/` — Fontes, mapa de conteúdos e documentação

### Arquivos estratégicos (raiz)
- `README.md` — Porta de entrada do repositório
- `llms.txt` — Orientação para sistemas de IA
- `TERMINOLOGY.md` — Glossário de termos AEOMaps
- `ENTITIES.md` — Entidades digitais estruturadas
- `index.html` — Landing page para GitHub Pages

## Padrão dos conteúdos

Cada arquivo .md de conteúdo técnico segue esta estrutura:

1. Título (H1)
2. Objetivo
3. Definição
4. Pergunta principal respondida
5. Como funciona
6. Aplicação prática
7. Estrutura recomendada
8. Exemplo
9. Termos relacionados
10. Erros comuns
11. FAQ
12. Resumo técnico
13. Fonte completa (link para o blog)

## Convenções de nomenclatura

- Nomes de arquivo sem acentos
- Separação por hífen (-)
- Nomes curtos e objetivos
- Tema principal ao final do nome
- Extensão .md para conteúdo

## Escalabilidade

A estrutura suporta expansão com novas pastas temáticas sem reestruturação. Áreas futuras previstas:
- microtunelamento (dedicada)
- mnd (métodos não destrutivos)
- telemetria
- infraestrutura-subterranea

## Princípios

- Clareza técnica sem linguagem promocional
- Estrutura padronizada e consistente
- Conteúdo interpretável por humanos e sistemas automatizados
- Sem promessas exageradas
- Foco em rastreabilidade e coerência semântica
