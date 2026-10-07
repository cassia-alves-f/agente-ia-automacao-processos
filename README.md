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

## O caminho até a solução

1. **Mapeamento:** documentação do processo em um guia passo a passo, junto com a gravação em vídeo da rotina completa.
2. **Primeira abordagem:** tradução da macro VBA de uma das etapas para Office Scripts, com um fluxo no Power Automate. O resultado foi validado contra a macro original, com 100% de correspondência nos totais.
3. **Mudança de rota:** a equipe concluiu que aquilo era uma automação, e não um agente, como o desafio pedia. O projeto passou a ser construído como um agente no Copilot Studio.
4. **Evolução do agente:** a lógica já validada foi levada para o agente, junto com novas instruções para uma conversa mais natural e para explicar os erros em português.

## Automação x agente

| | Automação (primeira abordagem) | Agente (versão final) |
| --- | --- | --- |
| Como funciona | Executa passos fixos | Conduz o processo e aplica as regras de negócio |
| Conferência | Feita depois, por uma pessoa | O agente confere os resultados e aponta alertas |
| Quando algo dá errado | Gera um erro técnico | Explica o erro em linguagem natural |
| Interação | Nenhuma | Conversa com quem usa |

## Resultados

- **Validação:** os resultados do agente bateram com os do processo manual.
- **Impacto estimado:** redução de cerca de 94% no tempo da tarefa.
- **Descobertas no caminho:** o agente revelou inconsistências nos dados que o processo antigo não tratava.

## Ferramentas

- Copilot Studio
- Office Scripts (TypeScript)
- Power Automate
- Excel

## Status

Projeto apresentado no Desafio de IA em outubro de 2026.
