# 🚀 JavaScript Fundamentals - Estudos Práticos

Este repositório foi criado com o objetivo de consolidar o aprendizado dos conceitos fundamentais do **JavaScript** (ES6+). Os exemplos práticos estão estruturados dentro de arquivos HTML, utilizando a tag `<script>` para execução direta no navegador através do console de desenvolvedor.

Inspirado nas aulas do canal *"Programador a bordo"*.

---

## 📂 Estrutura do Projeto

O projeto é dividido em arquivos temáticos para facilitar o estudo isolado de cada recurso da linguagem:

* **`index-variaveis.html`**: Declaração, atribuição e reatribuição de variáveis (`var`).
* **`operadores-matematicos.html`**: Operações aritméticas básicas, resto da divisão, exponenciação e operadores de incremento/decremento.
* **`strings.html`**: Manipulação de textos, propriedades, métodos nativos e Template Literals.
* **`booleanos.html`**: Tipos lógicos (`true`/`false`), operadores de comparação e igualdade estrita.
* **`operadores-logicos.html`**: Avaliação de valores *Truthy* e *Falsy*, negação lógica (`!`) e dupla negação (`!!`).

---

## 📝 Detalhamento dos Módulos e Códigos

### 1. Variáveis (index-variaveis.html)

Aborda a criação de variáveis na memória utilizando var, demonstrando a dinamicidade do JavaScript ao reatribuir novos valores e realizar operações simples.

```javascript

// console.log('Programador a bordo!');
var nome = 'Vitor Hugo';
console.log(nome); // Saída: 'Vitor Hugo'

var idade = 26;
console.log(idade); // Saída: 26

var total = idade + 10;
console.log(total); // Saída: 36 (26 + 10)

total = 50;
console.log(total); // Saída: 50 (Valor reatribuído)

total = 100;
console.log(total); // Saída: 100 (Nova reatribuição)

```
### 📂 2. Operadores Matemáticos (operadores-matematicos.html)

Explora os operadores aritméticos padrão, o operador de resto (módulo), exponenciação e a diferença crucial entre pré-incremento e pós-incremento.

``` JavaScript
// Operações básicas
console.log(10 + 5 + 3 + 4); // Saída: 22
console.log(50 - 10 - 5 + 2); // Saída: 37
console.log(5 * 5);           // Saída: 25
console.log(10 / 2);          // Saída: 5

// Exponenciação (Potência)
console.log(7 ** 2);          // Saída: 49 (7 elevado ao quadrado)

// Operações com variáveis
var a = 10;
var b = 18;
console.log(a + b);           // Saída: 28

// Módulo (Resto da divisão)
console.log(10 % 2);          // Saída: 0 (Divisão exata)
console.log(10 % 3);          // Saída: 1 (Sobram 1)
console.log(10 % 4);          // Saída: 2 (Sobram 2)

// Incrementos e Decrementos
var a = 1;
a = a + 1;
console.log(a);               // Saída: 2

a++;
console.log(a);               // Saída: 3

// Pós-incremento (Imprime primeiro, incrementa depois)
console.log(a++);             // Saída: 3 (Mas o valor interno virou 4)
console.log(a);               // Saída: 4

// Pré-incremento (Incrementa primeiro, imprime depois)
console.log(++a);             // Saída: 5

// Pré-decremento (Decrementa primeiro, imprime depois)
console.log(--a);             // Saída: 4

```
### 📂 3. Valores Booleanos e Comparações (booleanos.html)

Entendimento de lógica e tomadas de decisão através de operadores relacionais de comparação e testes de igualdade (ampla vs. estrita).


```JavaScript
var a = true;
console.log(a);               // Saída: true

var b = false;
console.log(b);               // Saída: false

// Operadores de Maior e Menor
console.log('3 < 5', 3 < 5);   // Saída: true
console.log('3 > 5', 3 > 5);   // Saída: false
console.log('5 >= 5', 5 >= 5); // Saída: true
console.log('5 >= 6', 5 >= 6); // Saída: false
console.log('5 <= 7', 5 <= 7); // Saída: true
console.log('5 <= 4', 5 <= 4); // Saída: false

// Operadores de Diferença e Igualdade
console.log('10 != 10', 10 != 10); // Saída: false
console.log('10 != 5', 10 != 5);   // Saída: true
console.log('4 == 4', 4 == 4);     // Saída: true
console.log('5 == 4', 5 == 4);     // Saída: false

// Comparação de Strings
var nome1 = 'vitor hugo';
var nome2 = 'Vitoriano';
console.log('nome1 == nome2', nome1 == nome2);   // Saída: false
console.log('nome1 != nome2', nome1 != nome2);   // Saída: true

// Igualdade Estrita (===) vs Igualdade Ampla (==)
console.log('4 === 4', 4 === 4);   // Saída: true (Mesmo valor e tipo)
console.log('4 == 4', 4 == 4);     // Saída: true
console.log("'4' === 4", '4' === 4); // Saída: false (Tipos diferentes: String vs Number)
console.log("'4' == 4", '4' == 4);   // Saída: true (Converte o tipo antes de comparar)

```

### 📂 4. Operadores Lógicos e Tipagem (operadores-logicos.html)


Estudo detalhado sobre comportamento lógico, negações e a descoberta do valor booleano intrínseco de dados do JavaScript através de regras de Truthy e Falsy.


```JavaScript
var a = true;
var b = false;

console.log(a);   // Saída: true
console.log(b);   // Saída: false

// Negação (!) e Dupla Negação (!!)
console.log(!a);  // Saída: false
console.log(!b);  // Saída: true

console.log('!!a', !!a); // Saída: true
console.log('!!b', !!b); // Saída: false

// Avaliação de Tipos Especiais e Valores Falsy/Truthy
// null
console.log(null);     // Saída: null
console.log(!null);    // Saída: true
console.log(!!null);   // Saída: false (Falsy)

// undefined
console.log(undefined);   // Saída: undefined
console.log(!undefined);  // Saída: true
console.log(!!undefined); // Saída: false (Falsy)

// String Vazia ('')
console.log('');       // Saída: vazio
console.log(!'');      // Saída: true
console.log(!!'');     // Saída: false (Falsy)

// Número Zero (0)
console.log(0);        // Saída: 0
console.log(!0);       // Saída: true
console.log(!!0);      // Saída: false (Falsy)

// Strings Preenchidas (Truthy)
console.log('texto');    // Saída: 'texto'
console.log(!'texto');   // Saída: false
console.log(!!'texto');  // Saída: true (Truthy)

```

### 📂 5. Manipulação de Strings (strings.html)


```JavaScript
var nome = 'Programador a bordo!';
console.log(nome); // Saída: 'Programador a bordo!'

// Propriedades e Métodos de Caixa
console.log(nome.length);        // Saída: 20 (Contagem de caracteres)
console.log('Programador'.length); // Saída: 11
console.log(nome.toUpperCase());  // Saída: 'PROGRAMADOR A BORDO!'
console.log(nome.toLowerCase());  // Saída: 'programador a bordo!'

// Métodos de Busca e Modificação
console.log(nome.indexOf('dor'));   // Saída: 8 (Posição inicial da substring)
console.log(nome.indexOf('teste')); // Saída: -1 (Não encontrado)
console.log(nome.replace('Programador', 'Desenvolvedor')); // Saída: 'Desenvolvedor a bordo!'
console.log(nome.slice(3, 8));     // Saída: 'grama' (Recorta do índice 3 ao 7)

// Manipulação de Espaços (trim)
var canalYoutube = '   Programador a bordo   ';
console.log(canalYoutube);        // Saída com os espaços originais
console.log(canalYoutube.trim()); // Saída: 'Programador a bordo' (Remove espaços das pontas)

// Concatenação de Textos
var autor = 'vitor hugo';

// Forma Antiga (+)
console.log('O canal do Youtube ' + canalYoutube.trim() + ' foi criado por ' + autor);

// Forma Moderna (Template Literals - Usando Crases ``)
console.log(`canal do Youtube ${canalYoutube.trim()} foi criado pelo ${autor}`);

```

🛠️ Como Executar o Projeto
Como o projeto utiliza estruturas puras contidas dentro de arquivos HTML, não é necessário instalar nenhum gerenciador de pacotes (como npm ou yarn).

1. Faça o clone deste repositório para sua máquina local:

   ```bash
   git clone [https://github.com/SEU-USUARIO/NOME-DO-REPOSITORIO.git](https://github.com/SEU-USUARIO/NOME-DO-REPOSITORIO.git)
   ```
2. Abra a pasta do projeto e dê um duplo clique sobre qualquer um dos arquivos .html (ex: strings.html) para abri-lo no seu navegador de preferência.

3. No navegador, pressione F12 (ou clique com o botão direito e selecione Inspecionar)

4. Vá até a aba Console para visualizar as saídas geradas pelos comandos console.log().

                                                           Desenvolvido para fins de estudo e prática de conceitos base do JavaScript. 💻✨