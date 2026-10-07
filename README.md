# Password Toggle

Um projeto simples e visualmente limpo para demonstrar a funcionalidade de mostrar ou ocultar a senha digitada em um campo de input.

## Objetivo

Esse projeto foi desenvolvido para praticar:

- manipulação do DOM com JavaScript
- eventos de clique
- alternância de tipo de input (`password` / `text`)
- uso de imagens como ícones de interface

## Funcionalidade

Ao clicar no ícone do olho, o usuário pode:

- ocultar a senha
- visualizar a senha digitada em tempo real
- alternar o ícone conforme o estado atual

É uma solução bem comum em formulários de login, cadastro e autenticação.

## 📁 Estrutura do projeto

```text
projeto02-password/
├── index.html
├── style.css
├── img/
│   ├── eye-close.png
│   └── eye-open.png
└── README.md
```

## 🛠️ Tecnologias utilizadas

- HTML5
- CSS3
- JavaScript

## 🔍 Como funciona

No arquivo `index.html`, existe um campo de senha e uma imagem que serve como botão de controle:

- quando o campo está em modo oculto, o valor aparece como `password`
- ao clicar no ícone, o JavaScript troca para `text`
- o ícone também muda para indicar que a senha está visível

A lógica principal está no script abaixo:

```javascript
let eyeicon = document.getElementById("eyeicon");
let password = document.getElementById("password");

eyeicon.onclick = function() {
    if(password.type == "password") {
        password.type = "text";
        eyeicon.src = "./img/eye-open.png";
    } else {
        password.type = "password";
        eyeicon.src = "./img/eye-close.png";
    }
}
```

## ▶️ Como executar

1. Abra a pasta do projeto no VS Code ou em qualquer editor.
2. Localize o arquivo `index.html`.
3. Abra-o no navegador.
4. Digite uma senha e clique no ícone do olho para alternar a visibilidade.

Você também pode usar a extensão Live Server para visualizar o projeto em tempo real no navegador.

## 🎨 Estilo visual

O design é simples e moderno, com:

- fundo roxo escuro
- caixa de input branca
- bordas arredondadas
- ícone clicável com boa visualização

---

<p align="center">
  Desenvolvido por <a href="https://github.com/LucMNS"><b>LucMNS</b></a>
</p>