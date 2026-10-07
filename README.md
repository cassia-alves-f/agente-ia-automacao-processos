# Agente de IA para Automação de Processos

Agente criado no Copilot Studio, no Desafio de IA da Renault Group Brasil, que assume de ponta a ponta a atualização diária de um sistema interno e reduz o tempo da tarefa em cerca de 94%.

**Este repositório é apenas documentação.** Por ser um projeto interno, não contém código, telas, bases nem dados da empresa.

## O problema

A atualização diária de um sistema interno, que alimenta um dashboard de acompanhamento, era feita manualmente por uma única pessoa. Todos os dias eram cinco bases de origens diferentes (sistemas, relatórios e e-mail), tratadas com macros, fórmulas e cópias, até a exportação manual dos arquivos XML carregados no sistema. A rotina levava cerca de 3 horas por dia, cerca de 750 horas por ano, dependia de uma pessoa e estava sujeita a erros.

## A solução

Criamos um agente no Copilot Studio que assume todo o processo. Mapeamos tudo o que a macro e as fórmulas faziam e ensinamos essas regras ao agente, por meio de instruções e de códigos de referência que ele mesmo executa. Integramos o agente a uma pasta do SharePoint da equipe, onde ficam as bases do dia e os arquivos de apoio, para que ele busque tudo sozinho. Assim, o agente faz o trabalho completo: localiza as bases, aplica as regras de cálculo, confere os resultados e gera os arquivos finais.

## Como funciona

1. A pessoa responsável salva as bases do dia na pasta do SharePoint e pede a atualização ao agente.
2. O agente busca os arquivos, faz todos os cálculos que antes eram manuais, confere os totais e aponta qualquer inconsistência.
3. O agente devolve os arquivos XML prontos para subir no sistema, explicando os alertas em linguagem simples.
4. A pessoa responsável confere e faz o upload, mantendo a validação humana antes de os dados chegarem à gestão.

A função de quem usa passa a ser só disponibilizar as bases e conferir o resultado. Todo o trabalho do meio fica com o agente.

## Resultados

- Os arquivos gerados pelo agente foram conferidos contra o processo manual: os XMLs saíram idênticos aos originais e os números bateram.
- O tempo estimado cai de cerca de 3 horas para cerca de 10 minutos por dia, uma redução de cerca de 94%:

| | Por dia | Por semana | Por mês | Por ano |
| --- | --- | --- | --- | --- |
| Antes (manual) | 3 h | 15 h | 63 h | 750 h |
| Com o agente | ~10 min | ~50 min | ~3,5 h | ~42 h |
| Economia | ~2h50 | ~14 h | ~59,5 h | ~708 h |

- O processo deixa de depender de uma única pessoa e passa a ter conferência automática todos os dias.

*Premissas: 21 dias úteis por mês e cerca de 250 por ano.*

## Próximos passos

Testar com a responsável pelo processo, implementar melhorias a partir do retorno dela e levar o mesmo modelo para outras rotinas da área.

## Ferramentas

- Copilot Studio
- SharePoint
- Excel
- VBA (análise da macro original)

## Status

Projeto apresentado no Desafio de IA em outubro de 2026.
