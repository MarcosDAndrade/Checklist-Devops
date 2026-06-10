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

💡 Exercício
Montar pipeline que: Instala dependências; Roda teste.

### 🔐 5. Trabalhar com Secrets
🎯 Objetivo:
Proteger dados sensíveis (tokens, senhas, etc.)

✅ Criar secret

✅ Usar no workflow

### ⚠️ Importante
Nunca dar `echo` em produção (vaza segredo nos logs)
Usar apenas quando necessário

### 📦 6. Upload de arquivos (Artifacts)
🎯 Objetivo: Salvar resultados do build/testes


## Resumo do que foi criado
|ID |Descrição | Demonstração |
|---|-----------|-------------|
|1- | Esse passo foi feito nas configurações do próprio github | |
|2- | Esse passo foi feito nas configurações do próprio github | |
|3- | Como todos os commits foram limitados a PRs,<br> decidi criar uma automação para todos os commits<br> que forem dados push,e independente da branch a action<br> faria um PR automaticamente com o titulo do commit em questão.| [Workflow PR Automático](https://github.com/MarcosDAndrade/Checklist-Devops/blob/main/.github/workflows/pipeline-pr-automatico.yml)|
|4- | Foi criado um workflow que busca um repositório existente, instala <br>as dependências para teste, executa o arquivo java e exibe o print da mensagem |[Workflow de execução](https://github.com/MarcosDAndrade/Checklist-Devops/blob/main/.github/workflows/pipeline-run-java.yml)|
|5- | Foi criado um workflow que lê a chave secret e exibe ela através do<br> comando 'echo' | [Usar secret key](https://github.com/MarcosDAndrade/Checklist-Devops/blob/main/.github/workflows/pipeline-secrets.yml) |
|6- | Foi criado um arquivo de teste para impressão de texto, e após o teste<br> foi implementada a mesma funcionalidade no workflow de execução java <br> para disponibilizar o download do resultado. | [Upload de arquivo](https://github.com/MarcosDAndrade/Checklist-Devops/blob/main/.github/workflows/pipeline-upload.yml)

## Prints
* Demonstação bloqueio de merge
  <img width="934" height="409" alt="image" src="https://github.com/user-attachments/assets/fedfb909-0545-4f4d-b283-ca5835636842" />
  
* Demonstração automação de PR:
  
  [Id de exemplo: 27221804242](https://github.com/MarcosDAndrade/Checklist-Devops/actions/runs/27221804242)

<img width="912" height="386" alt="image" src="https://github.com/user-attachments/assets/c44b65ae-41f3-4766-9828-c693dccd73f1" />

* Demonstração de execução de arquivo:
  
  [Id de exemplo: 80384132051](https://github.com/MarcosDAndrade/Checklist-Devops/actions/runs/27223443022/job/80384132051)
<img width="1080" height="454" alt="image" src="https://github.com/user-attachments/assets/7673f7de-2f77-43c8-8b7d-075961c21363" />

* Demonstração upload arquivos:
  
  [Id de exemplo: 27276651843](https://github.com/MarcosDAndrade/Checklist-Devops/actions/runs/27276651843)
<img width="1885" height="801" alt="Captura de tela 2026-06-10 094905" src="https://github.com/user-attachments/assets/9b958bd8-b442-4a54-8116-4ef3f1560125" />


