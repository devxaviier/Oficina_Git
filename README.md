<div align="center">

# Monitoria | Git & GitHub

**Exercícios resolvidos + automação com Shell Script**

![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)
![Shell Script](https://img.shields.io/badge/Shell_Script-121011?style=for-the-badge&logo=gnu-bash&logoColor=white)
![Status](https://img.shields.io/badge/status-concluído-success?style=for-the-badge)

*Do `git init` ao `git push`: tudo o que aprendi na oficina, em um só lugar.*

</div>

---

## Sobre o projeto

Este repositório reúne as atividades da **Oficina de Git & GitHub**: listas de exercícios das aulas 1, 2 e 3 (com respostas) e um script em Shell que automatiza o fluxo de envio de código, desenvolvido na aula 4.

**Período de realização:** Outubro de 2026.

> 💡 O objetivo é praticar o controle de versão e deixar o aprendizado documentado, versionado e acessível.

---

## 📂 Estrutura

```
Oficina_Git/
├── 📁 Atividades_Monitoria_GIT/
│   ├── 📝 Exercícios - Git & GitHub (Aula ...)
│   ├── 📝 Exercícios - Git & GitHub (Aula ...)
│   ├── 📝 Exercícios - Git & GitHub (Aula ...)
│   └── 📝 Exercícios - Git & GitHub (Aula ...)
├── 📄 README.md
└── ⚙️ enviar.sh
```

---

## O que cada aula cobre

| Aula | Tema | Conceitos |
|:---:|---|---|
| **1** | Introdução | `init`, `clone`, `add`, `commit`, `status`, `log`, hashes, HEAD, staging area, tags |
| **2** | Histórico, branches e envio | `log --oneline`, `branch`, `switch`, `merge`, `rebase`, `push`, `pull`, `tag` |
| **3** | Desfazendo erros e colaboração | `restore`, `reset`, `revert`, `reflog`, `commit --amend`, Fork e Pull Request |
| **4** | Automação | Script `.sh` com `add`, `commit` e `push` |

---

## Aula 4 | O script `enviar.sh`

Script em Shell que automatiza o fluxo de envio de alterações ao GitHub (add, commit e push) com um único comando:

```bash
#!/bin/bash
# Para indicar que o script deve ser executado pelo Bash :)

git add .
git commit -m "Atualizando arquivos do projeto"
git push
```

### Como usar

```bash
# 1. Dar permissão de execução (só na primeira vez)
chmod +x enviar.sh

# 2. Rodar o script
./enviar.sh
```

O commit sempre usa a mensagem **"Atualizando arquivos do projeto"**.

### O que acontece por baixo dos panos

```
git add .      →  coloca as alterações na staging area
git commit -m  →  registra o commit com a mensagem
git push       →  envia para o GitHub
```

---

## Resumo rápido dos comandos

<details>
<summary><b>🔧 Básicos</b></summary>

| Comando | O que faz |
|---|---|
| `git init` | Inicia um repositório |
| `git clone <url>` | Copia um repositório remoto |
| `git status` | Mostra o estado dos arquivos |
| `git add .` | Adiciona tudo à staging area |
| `git commit -m "msg"` | Registra um commit |
| `git log --oneline` | Histórico resumido |

</details>

<details>
<summary><b>🌿 Branches</b></summary>

| Comando | O que faz |
|---|---|
| `git branch nome` | Cria uma branch |
| `git switch -c nome` | Cria e troca para a branch |
| `git merge nome` | Integra uma branch na atual |
| `git rebase main` | Reaplica commits sobre a main |

</details>

<details>
<summary><b>⏪ Desfazendo coisas</b></summary>

| Comando | O que faz |
|---|---|
| `git restore arquivo` | Descarta alterações locais |
| `git reset --soft HEAD~1` | Desfaz o commit, mantém na staging |
| `git reset --hard HEAD~1` | Desfaz o commit e descarta tudo |
| `git revert HEAD` | Cria um commit que desfaz o último |
| `git reflog` | Mostra as movimentações do HEAD |

</details>

<details>
<summary><b>🤝 Colaboração</b></summary>

**Fluxo de trabalho:** Fork → Clone → Branch → Commit → Push → Pull Request → Revisão → Merge → Sync

</details>

---

## Tecnologias

- **Git** — controle de versão
- **GitHub** — hospedagem e colaboração
- **Bash** — automação de tarefas
- **Markdown** — documentação

---

## Autor

**Theo Xavier**
Estudante de Engenharia de Software no CEUB

| | |
|---|---|
| **RA:** | `22650114` |
| **E-mail institucional:** | [theo.xavier@sempreceub.com](theo.xavier@sempreceub.com) |
| | |

[![GitHub](https://img.shields.io/badge/GitHub-devxaviier-181717?style=flat-square&logo=github)](https://github.com/devxaviier)

---

<div align="center">

Obrigado por visitar meu repositório, é um prazer te ter por aqui!

Espero que este conteúdo seja útil para seus estudos. Se te ajudou, considere deixar uma ⭐ para apoiar o projeto.


</div>
