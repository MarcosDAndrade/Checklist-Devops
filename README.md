# Checklist-Devops

### ✅ Checklist DevOps – GitHub Actions (Iniciante)

### 🔒 1. Bloquear commits diretos na `main`

🎯 Objetivo
Garantir que ninguém faça push direto — tudo deve passar por PR.

### 🔁 2. Exigir aprovação de PR para merge

🎯 Objetivo
Implementar fluxo correto de revisão.

✅ O que fazer
Já dentro da rule criada:

🚫 Require pull request reviews before merging

Definir: 1 ou mais aprovadores

### ⚙️ 3. Criar e usar GitHub Actions

🎯 Objetivo: Criar pipelines automáticos.

### ♻️ 4. Reaproveitar Actions do marketplace

🎯 Objetivo: Evitar reinventar roda.

## Resumo do que foi criado
|ID |Descrição | Demonstração |
|---|-----------|-------------|
|1- | Esse passo foi feito nas configurações do próprio github | |
|2- | Esse passo foi feito nas configurações do próprio github | |
|3- | Como todos os commits foram limitados a PRs,<br> decidi criar uma automação para todos os commits<br> que forem dados push,e independente da branch a action<br> faria um PR automaticamente com o titulo do commit em questão.| [Workflow PR Automático](https://github.com/MarcosDAndrade/Checklist-Devops/blob/main/.github/workflows/pipeline-pr-automatico.yml)|
|4- | 


## Prints

* Demonstração automação de PR

[Id de exemplo: 27221804242](https://github.com/MarcosDAndrade/Checklist-Devops/actions/runs/27221804242)

<img width="912" height="386" alt="image" src="https://github.com/user-attachments/assets/c44b65ae-41f3-4766-9828-c693dccd73f1" />

