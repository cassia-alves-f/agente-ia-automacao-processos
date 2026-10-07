# Agente de IA para Automação de Processos

Agente de IA criado no Copilot Studio, no Desafio de IA da Renault Group Brasil, que substituiu uma macro VBA na atualização diária de um sistema interno e reduziu o tempo da tarefa em cerca de 94%.

**Este repositório é apenas documentação.** Por ser um projeto interno, não contém código, telas, bases nem dados da empresa.

## O desafio

O Desafio de IA da Renault Group Brasil é uma competição interna entre equipes, com uma fase de onboarding e aprendizado. O requisito era criar um agente de IA para melhorar uma tarefa da área. Escolhemos uma rotina diária que tomava muito tempo do nosso time.

## O problema

A atualização diária do sistema era feita manualmente, com apoio de uma macro VBA que só rodava com alguém abrindo o arquivo no computador. A rotina envolvia várias bases de dados, cálculos, fórmulas e geração de arquivos, dependia de uma única pessoa e estava sujeita a erros manuais.

## O que o agente faz

O agente conduz o processo de ponta a ponta:

- Trata os dados
- Aplica as regras de negócio
- Confere os resultados
- Aponta alertas quando algo foge do esperado
- Explica os erros em linguagem natural
- Gera os arquivos finais

A equipe fica só com a revisão final.

## Como foi construído

1. **Mapeamento:** documentação do processo em um guia passo a passo, junto com a gravação em vídeo da rotina completa.
2. **Análise da macro:** leitura da macro VBA para entender exatamente o que ela fazia em cada etapa.
3. **Desenvolvimento do agente:** o processo e a lógica da macro foram transformados em instruções para um agente no Copilot Studio, que passou a executar a rotina completa, conversando de forma natural com quem usa e explicando os erros em português.

## Resultados

- **Validação:** os resultados do agente bateram com os do processo manual.
- **Impacto estimado:** redução de cerca de 94% no tempo da tarefa.
- **Descobertas no caminho:** o agente revelou inconsistências nos dados que o processo antigo não tratava.

## Ferramentas

- Copilot Studio
- Excel
- VBA (análise da macro original)

## Status

Projeto apresentado no Desafio de IA em outubro de 2026.
