# 🎯 Jogo do Número Secreto

Um jogo simples e interativo desenvolvido em **JavaScript**, onde o jogador precisa adivinhar um número secreto gerado aleatoriamente.

O projeto utiliza manipulação de DOM, lógica condicional, controle de tentativas e **síntese de voz** com a biblioteca ResponsiveVoice para tornar a experiência mais dinâmica.

---

## 🚀 Funcionalidades

- 🔢 Geração de número aleatório
- 🔁 Controle para não repetir números já sorteados
- 📊 Contador de tentativas
- 🔊 Feedback por voz (Text-to-Speech)
- 🔄 Botão para reiniciar o jogo
- 💡 Dicas informando se o número secreto é maior ou menor

---

## 🛠️ Tecnologias utilizadas

- HTML5
- CSS3
- JavaScript (Vanilla JS)
- ResponsiveVoice.js (para narração por voz)

---

## 🎮 Como funciona o jogo

1. O sistema gera um número aleatório.
2. O jogador digita um número no campo de entrada.
3. O sistema informa se:
   - ✅ Acertou
   - ⬆️ O número secreto é maior
   - ⬇️ O número secreto é menor
4. O jogo contabiliza o número de tentativas.
5. Ao acertar, o botão **Reiniciar** é habilitado.

---

## 📂 Estrutura do Projeto

📁 jogo-numero-secreto
├── index.html
├── style.css
└── app.js---

## 🧠 Lógica Principal

### Variáveis Globais

```javascript
let listaDeNumerosSorteados = [];
let numeroLimite = 50;
let numeroSecreto = gerarNumeroAleatorio();
let tentativas = 1;