# Atividade Prática – Versionamento de Código com Git e GitHub

## Objetivo
Praticar as principais ferramentas de versionamento de código utilizadas no mercado de trabalho, aplicando conceitos de Git e GitHub em um projeto desenvolvido em dupla.

---

## Ferramentas Necessárias
Antes de iniciar, ambos os integrantes devem instalar e configurar:
* **Git** (Instalado na máquina)
* **Git Bash** (Terminal utilitário)
* **VS Code** (Editor de código)
* **Conta ativa no GitHub**

---

## Organização da Dupla
* **Integrante 1:** Responsável por criar o repositório inicial e desenvolver a página Home (`index.html`).
* **Integrante 2:** Responsável por documentar o processo e desenvolver a página Login (`login.html`).

---

## Passo a Passo para Execução da Atividade

### Parte 1 – Criação do Projeto (Integrante 1)
1. Crie uma pasta chamada `atividade-versionamento`.
2. Abra esta pasta no VS Code.
3. Abra o Git Bash dentro da pasta.
4. Inicialize o repositório Git local:
   ```bash
   git init
   ```
5. Crie manualmente dois arquivos vazios na raiz: `index.html` e `login.html`.
6. Realize o primeiro commit do projeto estruturado:
   ```bash
   git add .
   git commit -m "Projeto inicial"
   ```

### Parte 2 – Conexão com o GitHub (Integrante 1)
1. Acesse o seu perfil no GitHub.
2. Crie um novo repositório com o nome de sua preferência.
3. **Atenção:** Não marque a opção de adicionar arquivo README automaticamente.
4. Clique em "Create repository".
5. Conecte o repositório local ao remoto (substitua pela sua URL):
   ```bash
   git remote add origin URL_DO_REPOSITORIO
   ```
6. Renomeie a branch principal e envie o código:
   ```bash
   git branch -M main
   git push -u origin main
   ```

### Parte 3 – Clonagem do Projeto (Integrante 2)
1. Copie a URL do repositório remoto criado pelo Integrante 1.
2. Abra o Git Bash no seu computador.
3. Navegue até a pasta onde deseja salvar o projeto.
4. Clone o repositório:
   ```bash
   git clone URL_DO_REPOSITORIO
   ```
5. Abra a pasta do projeto clonado utilizando o VS Code.

### Parte 4 – Criação das Branches (Ambos Integrantes)
Cada integrante deve criar e entrar em sua própria branch de trabalho pelo terminal:

* **Integrante 1 (Branch Home):**
  ```bash
  git checkout -b home
  ```
* **Integrante 2 (Branch Login):**
  ```bash
  git checkout -b login
  ```
* **Para verificar se você está na branch correta, digite:**
  ```bash
  git branch
  ```

### Parte 5 – Desenvolvimento do Código

#### Integrante 1 (Desenvolvimento da Home)
Insira o seguinte código dentro do arquivo `index.html`:
```html
<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <title>Home</title>
</head>
<body>
    <h1>Bem-vindo ao sistema!</h1>
</body>
</html>
```
Após salvar o arquivo, envie as alterações para o GitHub:
```bash
git add .
git commit -m "Criação da página Home"
git push origin home
```

#### Integrante 2 (Desenvolvimento do Login)
Insira o seguinte código dentro do arquivo `login.html`:
```html
<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <title>Login</title>
</head>
<body>
    <h1>Tela de Login</h1>
    <form action="index.html">
        <input type="text" placeholder="Usuário">
        <input type="password" placeholder="Senha">
        <button type="submit">Entrar</button>
    </form>
</body>
</html>
```
Após salvar o arquivo, envie as alterações para o GitHub:
```bash
git add .
git commit -m "Criação da página Login"
git push origin login
```

### Parte 6 – Integração e Merge das Branches (No GitHub)
Depois que ambos derem o `push` em suas respectivas branches, sigam os passos no site do GitHub:
1. Acesse a página do repositório no GitHub.
2. Abra um **Pull Request** da branch `home` direcionado para a branch `main`.
3. Aprove e faça o **Merge** desse Pull Request.
4. Abra um novo **Pull Request** da branch `login` direcionado para a branch `main`.
5. Aprove e faça o **Merge** deste último também.

### Parte 7 – Atualização Local do Projeto (Ambos Integrantes)
Para sincronizar as atualizações finais feitas no GitHub de volta para o seu computador, execute no Git Bash:
```bash
git checkout main
git pull origin main
```

---

## Resultado Esperado
* Ao abrir o arquivo `login.html` no navegador, a tela de login deve carregar.
* Ao preencher os dados e clicar em **Entrar**, o usuário deve ser redirecionado para a página `index.html` (Home).

---

## Itens a Serem Entregues
1. **Link do Repositório:** URL pública do GitHub contendo todo o histórico de commits da dupla.
2. **Documento de Acompanhamento (Feito pelo Integrante 2):** PDF ou relatório contendo histórico de comandos utilizados, prints das telas, explicações de cada etapa, além de problemas encontrados e soluções aplicadas.
3. **Projeto Sincronizado:** Código final rodando perfeitamente integrado na branch `main`.

---

## Critérios de Avaliação

| Critério | Pontuação Máxima |
| :--- | :---: |
| Criação correta do repositório local | 2 Pontos |
| Utilização correta do GitHub remoto | 2 Pontos |
| Uso correto de branches separadas | 2 Pontos |
| Histórico de commits realizados pela dupla | 2 Pontos |
| Integração das páginas e documentação final | 2 Pontos |
| **Total** | **10 Pontos** |
