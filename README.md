Documento de Acompanhamento – Atividade Prática de Versionamento de Código com Git e GitHub

Dupla: Kayke Debora

Turma: 3°A Desenvolvimento de sistemas

Disciplina: Versionamento de Código

---

Objetivo

O objetivo desta atividade foi aprender a utilizar o Git e o GitHub para realizar o versionamento de código em equipe, utilizando branches, commits, push, pull e merge durante o desenvolvimento de um projeto simples.

---

Etapa 1 – Criação do Projeto

Primeiro foi criada a pasta atividade-versionamento e ela foi aberta no Visual Studio Code. Em seguida, foi inicializado um repositório Git utilizando o comando "git init". Depois foram criados os arquivos "index.html" e "login.html", adicionados ao Git e realizado o primeiro commit.

Comandos utilizados

git init
git add .
git commit -m "Projeto inicial"

---

Etapa 2 – Criação do Repositório no GitHub

Foi criado um novo repositório no GitHub sem arquivo README. Depois o repositório local foi conectado ao repositório remoto utilizando a URL fornecida pelo GitHub. Por fim, os arquivos foram enviados para o GitHub.

Comandos utilizados

git remote add origin https://github.com/kakamn2505/batatafrita.git
git branch -M Main
git push -u origin Main

---

Etapa 3 – Clonagem do Projeto

O segundo integrante clonou o repositório utilizando o comando "git clone" e abriu o projeto no Visual Studio Code para iniciar o desenvolvimento.

Comando utilizado

git clone https://github.com/kakamn2505/batatafrita.git

---

Etapa 4 – Criação das Branches

Cada integrante criou sua própria branch para trabalhar separadamente. Um integrante criou a branch "Debora" e o outro criou a branch "kaiak".

Comandos utilizados

git checkout -b Debora
git checkout -b Kaiak
git branch

---

Etapa 5 – Desenvolvimento

Cada integrante desenvolveu sua parte do projeto.

- O Integrante 1 criou a página Home. (Debora)
- O Integrante 2 criou a página Login. (Kaiak)

Após finalizar as alterações, cada um realizou um commit e enviou sua branch para o GitHub.

Comandos utilizados

git add .
git commit -m "Criação da página Home"
git push origin Debora

git add .
git commit -m "Criação da página Login"
git push origin Kaiak

---

Etapa 6 – Merge das Branches

Após finalizar o desenvolvimento, foram criados Pull Requests no GitHub para unir as branches "Debora" e "Kaiak" à branch "Main". Depois os merges foram realizados.

---

Etapa 7 – Atualização do Projeto

Depois do merge, o projeto foi atualizado utilizando o comando abaixo para baixar as alterações da branch principal.

Comandos utilizados

git checkout Main
git pull origin Main

---

Todos os comandos utilizados

git init
git add .
git commit -m "Projeto inicial"

git remote add origin https://github.com/kakamn2505/batatafrita.git
git branch -M Main
git push -u origin Main

git clone https://github.com/kakamn2505/batatafrita.git

git checkout -b Debora
git checkout -b Kaiak

git branch

git add .
git commit -m "Criação da página Home"
git push origin Debora

git add .
git commit -m "Criação da página Login"
git push origin Kaiak

git checkout Main
git pull origin Main

---

Dificuldades encontradas

Durante a atividade tivemos algumas dificuldades para utilizar os comandos do Git corretamente e entender como funcionam as branches. Também houve atenção na hora de enviar as alterações para o GitHub e realizar o merge sem erros.

---

Soluções adotadas

Conferimos os comandos antes de executá-los, verificamos se estávamos na branch correta e utilizamos o GitHub para realizar os Pull Requests e os merges. Após isso, atualizamos o projeto com "git pull" para que todos tivessem a versão mais recente.

---

Conclusão

A atividade foi importante para aprender como funciona o versionamento de código utilizando Git e GitHub. Foi possível praticar o trabalho em equipe, a criação de branches, os commits, o envio das alterações para o GitHub e o merge entre diferentes versões do projeto. Esses conhecimentos são muito utilizados no desenvolvimento de software e serão úteis em projetos futuros.
