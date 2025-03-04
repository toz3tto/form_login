# 📌 Documentação - Página de Login

## 📖 1. Visão Geral
Este repositório contém os arquivos de uma **página de login** estilizada com CSS. A página permite que o usuário insira suas credenciais e envie os dados via formulário.

---
### 🎥 Demonstração


https://github.com/user-attachments/assets/e2f3a8d9-2fc8-4a4c-9e60-55e8428ff4f8


---


### 📂 Estrutura do Projeto:
```
📁 projeto-login/
│── 📄 index.html  → Estrutura HTML do login
│── 🎨 login.css   → Estilização da página
```

---

## 🏗 2. Estrutura do `index.html`

### 🔹 Declaração Inicial
```html
<!DOCTYPE html>
<html lang="pt-br">
```
- Define o documento como **HTML5**.
- Especifica o idioma como **português do Brasil**.

### 🔹 Cabeçalho da Página
```html
<head>
    <meta charset="UTF-8">
    <title>Login</title>
    <link rel="stylesheet" href="login.css">
</head>
```
- **Codificação UTF-8** para suporte a caracteres especiais.
- **Título da página** `"Login"`.
- **Importação do CSS** para estilização.

---

## 📝 3. Corpo do HTML

### 🔹 Estrutura do Formulário
```html
<body>
    <form action="#" method="get">
        <fieldset>
            <legend>LOGIN</legend>
            <label for="usuario">Usuário</label>
            <input type="text" id="usuario" required autofocus>

            <label for="senha">Senha</label>
            <input type="password" id="senha" required>

            <div class="actions">
                <input type="reset" value="Apagar" class="btn2 btn--apagar">
                <input type="submit" value="Entrar" class="btn2">
            </div>
        </fieldset>
    </form>
</body>
```
- **`<fieldset>`**: Agrupa os elementos do formulário.
- **`<legend>`**: Define o título "LOGIN".
- **`<label>`**: Descreve os campos de entrada.
- **`<input>`**: Campos obrigatórios para usuário e senha.
- **Botões**:  
  ✅ `"Apagar"` → Limpa os campos.  
  ✅ `"Entrar"` → Envia os dados preenchidos.

---

## 🎨 4. Estilização `login.css`

### 🔹 Configurações Gerais
```css
html {
    background-color: #649484;
    font-family: "Helvetica Neue", Arial, sans-serif;
}
body {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    min-height: 100vh;
    margin: 0;
}
```
- Define um **fundo verde suave**.
- Utiliza a **fonte Helvetica**.
- Centraliza o conteúdo.

### 🔹 Estilização do Formulário
```css
form {
    width: 350px;
    background-color: #dee1e1;
    border-radius: 5px;
    box-shadow: 3px 3px 10px #333;
    padding: 1em;
}
```
- **Largura fixa** de 350px.
- **Bordas arredondadas**.
- **Sombra** para efeito 3D.

### 🔹 Campos de Entrada
```css
input {
    padding: .75em;
    border-radius: 5px;
    border: 1px solid #bbb;
    font-size: 1em;
}
```
- **Bordas arredondadas**.
- **Fonte responsiva**.

### 🔹 Botões
```css
.btn {
    background-color: rgb(100, 100, 217);
    color: white;
    cursor: pointer;
}
.btn--apagar {
    background-color: rgb(236, 72, 96);
}
```
- Cores personalizadas para os botões de ação.

---

## 🚀 5. Melhorias e Sugestões
✅ **Alterar `method="post"`** para maior segurança.  
✅ **Definir um `action` real** para processar login.  
✅ **Adicionar validação JavaScript** para experiência aprimorada.  


