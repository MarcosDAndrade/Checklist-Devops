# Checklist-Devops

✅ Checklist DevOps – GitHub Actions (Iniciante)

🔒 1. Bloquear commits diretos na `main`

🎯 Objetivo
Garantir que ninguém faça push direto — tudo deve passar por PR.

## Resumo do que foi criado
|ID |Descrição | Demonstração |
|---|-----------|-------------|
|1-| Como todos os commits foram limitados a PRs,<br> decidi criar uma automação para todos os commits<br> que forem dados push,e independente da branch a action<br> faria um PR automaticamente com o titulo do commit em questão.| [Workflow PR Automático](https://github.com/MarcosDAndrade/Checklist-Devops/blob/main/.github/workflows/pipeline-pr-automatico.yml) | |
|2- | Para não ficar revisando todos os PRs, criei uma função que aprova<br> todas as alterações que são feitas em uma branch confiável | [Workflow de aprovação automática](https://github.com/MarcosDAndrade/Checklist-Devops/blob/main/.github/workflows/pipeline-aprovar-pr.yml) |


## Prints

* Demonstração automação de PR

[Id de exemplo: 27221804242](https://github.com/MarcosDAndrade/Checklist-Devops/actions/runs/27221804242)


