# Projeto de Prática - GitHub Projects e Branches

Este repositório é utilizado na atividade prática de GitHub Projects, Issues, Branches e Pull Requests.

## 📝 Instruções

Cada aluno deve:

✅ Criar sua própria branch seguindo o padrão: `feature-nomeAluno`  
✅ Criar um arquivo `README.md` com a ideia do seu projeto fictício ou real  
✅ Fazer um Pull Request para a branch `main`  
✅ Aguardar a análise e aprovação do professor  




## 🎯 Objetivo


Praticar:

- Criação de Branches
- Edição de README.md
- Pull Requests
- Uso de GitHub Projects para organizar as tarefas


### 1. Clonar o repositório

```bash
# Clonar o repositório
git clone https://github.com/seu-usuario/github-projects-pratica.git
cd github-projects-pratica

# Atualizar o repositório
git checkout main
git pull origin main

# Criar e acessar sua branch
git checkout -b feature/seuNome

# Criar pasta e README
mkdir seuNome
cd seuNome
touch README.md

# Adicionar, commitar e subir
git add .
git commit -m "feat: adiciona pasta e README do projeto do SeuNome"
git push origin feature/seuNome

# Atualizar o repositório depois
git checkout main
git pull origin main
git checkout feature/seuNome
git merge main
