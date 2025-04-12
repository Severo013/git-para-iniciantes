# 📘 Apostila Básica de Git para Iniciantes

Bem-vindo(a)! 👋 Este material foi preparado para te ajudar a entender os conceitos fundamentais do Git e te dar confiança para começar a usar essa ferramenta no seu dia a dia com código e projetos colaborativos!

---

## 🧠 O que é o Git?

O **Git** é um sistema de controle de versões. Ele te ajuda a:

- Salvar diferentes versões do seu projeto 📁
- Trabalhar em equipe sem bagunça 👥
- Voltar no tempo caso algo dê errado 🔙

---

## 📦 Repositório

Um **repositório** é onde o Git guarda todos os arquivos e o histórico de versões do seu projeto.

- Pode ser **local** (na sua máquina)
- Pode ser **remoto** (ex: GitHub 🌐)

🛠 Para criar um repositório:
```bash
git init   # Cria um repositório local
```

🛰 Para clonar um repositório remoto:
```bash
git clone https://github.com/usuario/repositorio.git
```

---

## 🌿 Branch (Ramos)

Uma **branch** é uma linha de desenvolvimento paralela. Você pode experimentar sem afetar a versão principal!

- `main` (ou `master`) é normalmente a branch principal

📌 Comandos úteis:
```bash
git branch              # Lista as branches
git checkout -b nova-feature   # Cria e muda para nova branch
```

---

## 💾 Commit

Um **commit** salva uma versão do projeto. É como tirar uma foto do estado atual dos arquivos. 🖼️

📌 Para fazer um commit:
```bash
git add .               # Adiciona todos os arquivos alterados
# ou git add nome-do-arquivo.ext

git commit -m "Mensagem explicando o que foi feito"
```

💡 Dica: escreva mensagens de commit claras, ex: `Corrige bug na tela de login`

---

## 🔄 git fetch, pull e push

### 📥 `git fetch`

Busca atualizações do repositório remoto, mas **não altera nada ainda**:
```bash
git fetch
```

### 📤 `git pull`

Atualiza seu repositório local com as alterações remotas (faz o `fetch` + `merge`):
```bash
git pull
```

### 🚀 `git push`

Envia suas alterações para o repositório remoto (ex: GitHub):
```bash
git push origin nome-da-branch
```

🔐 Importante: você precisa ter permissão para enviar para o repositório!

---

## ⏪ git revert

Fez algo errado? O `git revert` cria um novo commit que desfaz um commit anterior **sem apagar o histórico**:

```bash
git revert <hash-do-commit>
```

📝 Dica: use `git log` para encontrar o hash do commit:
```bash
git log
```

---

## 🍴 O que é um Fork?

Um **fork** é uma cópia de um repositório no seu próprio GitHub. Você pode usar isso para:

- Sugerir melhorias em projetos de outras pessoas 🛠️
- Criar sua própria versão de um projeto público 📂

🔗 Como funciona o fluxo com fork:

1. Clique em **Fork** no repositório original no GitHub
2. O repositório será copiado para a sua conta
3. Faça alterações no seu fork
4. Crie um **Pull Request** para o repositório original

---

## ⚔️ Conflitos no Git (Merge Conflicts)

Os **conflitos** acontecem quando duas pessoas alteram a mesma parte do código em branches diferentes. O Git não sabe qual mudança deve ficar.

🧯 Como resolver:

1. O Git vai mostrar o arquivo com conflitos marcado assim:
```txt
<<<<<<< HEAD
Seu código
=======
Código da outra branch
>>>>>>> outra-branch
```

2. Edite o arquivo escolhendo o que deve ficar ✅
3. Salve o arquivo e faça o commit normalmente:
```bash
git add nome-do-arquivo

git commit -m "Resolve conflito no arquivo X"
```

💡 Dica: quanto mais frequente o `pull`, menos chances de conflito!

---

## ✅ Dicas Finais

- Use `git status` para ver o que está acontecendo no repositório ✅
- Trabalhe em branches para testar ideias sem medo 💡
- Commit frequentemente com mensagens claras 📬
- Não tenha medo de explorar! Git é prática! 💪

---

## 💬 Dúvidas?
Se você tiver alguma dúvida, peça ajuda! Todos estamos aqui para aprender juntos. 😊

---

Bons commits e pull requests! 🚀

