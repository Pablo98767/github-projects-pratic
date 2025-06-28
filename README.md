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




# Guia de Fluxo do Git para Projetos de Software

Este guia explica o fluxo básico de trabalho com Git em projetos de software, incluindo como criar uma branch, realizar alterações, subir mudanças, criar um pull request, fazer pull e usar o stash.

---

## 1. Clonar o Repositório

Se você ainda não possui o repositório localmente, pode cloná-lo com o comando:

```bash
git clone <url-do-repositorio>
```

Substitua `<url-do-repositorio>` pela URL do repositório remoto.

---

## 2. Criar uma Nova Branch

Antes de começar a trabalhar em uma nova funcionalidade ou correção de bug, crie uma branch para suas alterações:

```bash
git checkout -b nome-da-branch
```

- Substitua `nome-da-branch` por um nome descritivo, como `feature/nova-funcionalidade` ou `bugfix/corrigir-erro`.

---

## 3. Fazer Alterações no Código

Realize as alterações necessárias no código. Após isso, você pode verificar o status do repositório para ver os arquivos modificados:

```bash
git status
```

---

## 4. Adicionar Arquivos ao Staging

Adicione os arquivos modificados ao staging para preparar o commit:

```bash
git add <arquivo>
```

Ou adicione todos os arquivos modificados:

```bash
git add .
```

---

## 5. Fazer um Commit

Depois de adicionar os arquivos ao staging, faça um commit para salvar as alterações localmente:

```bash
git commit -m "Mensagem descritiva do commit"
```

Certifique-se de que a mensagem do commit descreva claramente as alterações realizadas.

---

## 6. Subir a Branch para o Repositório Remoto

Envie sua branch para o repositório remoto:

```bash
git push origin nome-da-branch
```

---

## 7. Criar um Pull Request (PR)

Após subir a branch, vá até a interface do repositório no GitHub, GitLab ou outra plataforma de controle de versão e crie um Pull Request (PR).

- Certifique-se de selecionar a branch correta para merge (geralmente `main` ou `develop`).
- Adicione uma descrição detalhada do que foi feito na branch.

---

## 8. Fazer Pull para Atualizar o Código Local

Para sincronizar o código local com as alterações do repositório remoto, use o comando:

```bash
git pull
```

Isso baixa as alterações do repositório remoto e as mescla com sua branch atual.

---

## 9. Usar o Stash (Opcional)

Se você estiver trabalhando em algo e precisar mudar de branch sem perder suas alterações, use o stash:

### Salvar Alterações no Stash
```bash
git stash
```

### Verificar o Stash
```bash
git stash list
```

### Recuperar Alterações do Stash
```bash
git stash apply
```

### Remover Alterações do Stash Após Aplicá-las
```bash
git stash drop
```

---

## 10. Mesclar o Pull Request

Após revisão e aprovação do Pull Request, faça o merge na branch principal (`main` ou `develop`). Isso geralmente é feito na interface da plataforma de controle de versão.

---

## 11. Deletar a Branch (Opcional)

Depois que a branch for mesclada, você pode deletá-la para manter o repositório limpo:

### Deletar a Branch Localmente
```bash
git branch -d nome-da-branch
```

### Deletar a Branch no Repositório Remoto
```bash
git push origin --delete nome-da-branch
```

---

## Resumo dos Comandos

1. `git checkout -b nome-da-branch` - Criar uma nova branch.
2. `git add <arquivo>` ou `git add .` - Adicionar arquivos ao staging.
3. `git commit -m "Mensagem do commit"` - Fazer commit das alterações.
4. `git push origin nome-da-branch` - Subir a branch para o remoto.
5. `git pull` - Atualizar o código local.
6. `git stash` - Salvar alterações no stash.
7. `git stash apply` - Recuperar alterações do stash.
8. `git branch -d nome-da-branch` - Deletar branch localmente.
9. `git push origin --delete nome-da-branch` - Deletar branch no remoto.

---

Este fluxo cobre as operações mais comuns no Git para colaborar em projetos de software. Certifique-se de seguir as práticas recomendadas da equipe e da organização ao trabalhar em um repositório compartilhado.
