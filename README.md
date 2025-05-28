# 🎓 Desafios JavaScript: Palíndromos e Boletim Escolar

Este repositório contém a resolução de dois desafios didáticos para praticar conceitos fundamentais de JavaScript:

1. 🧠 **Verificador de Palíndromos**
2. 📊 **Aplicativo de Boletim Escolar (Cálculo de Média)**

---

## 1. 🧠 Verificador de Palíndromos

### Objetivo

Criar um app interativo que verifica se uma palavra ou frase é um **palíndromo** — ou seja, se pode ser lida da mesma forma da esquerda para a direita e vice-versa, ignorando espaços, pontuação e maiúsculas/minúsculas.

### Funcionalidades

- Input com `id="text-input"`
- Botão com `id="check-btn"`
- Exibição do resultado em `#result`
- Alerta quando o campo estiver vazio
- Exemplo:  
  Entrada: `race car`  
  Saída: `race car is a palindrome.`

### Tecnologias Usadas

- HTML5
- CSS3 (estilização simples)
- JavaScript (DOM + lógica de string)

### Estrutura de Arquivos

/palindrome-checker/

├── index.html

├── styles.css

└── script.js

kotlin
Copy
Edit

---

## 2. 📊 Construindo um Aplicativo de Boletim Escolar

### Objetivo

Desenvolver uma função chamada `getAverage(scores)` que recebe um array com as notas dos alunos e retorna a média aritmética da turma.

### Desafio Original

```js
function getAverage(scores) {
  const sum = scores.reduce((acc, score) => acc + score, 0);
  return Math.round((sum / scores.length) * 10) / 10;
}

console.log(getAverage([92, 88, 12, 77, 57, 100, 67, 38, 97, 89])); // 71.7
console.log(getAverage([45, 87, 98, 100, 86, 94, 67, 88, 94, 95])); // 85.4
