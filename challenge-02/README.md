# Desafio da semana #2

Nesse exercício, você está livre para escolher os nomes para suas variáveis e funções! :smile:

```js
// Crie uma função que receba dois argumentos e retorne a soma dos mesmos.
function soma(argument1, argument2) { return argument1 + argument2 };

// Declare uma variável que receba a invocação da função criada acima, passando dois números quaisquer por argumento, e somando `5` ao resultado retornado da função.
var resultadoCinco = soma(2, 3) + 5;

// Qual o valor atualizado dessa variável?
10

// Declare uma nova variável, sem valor.
var semValor;

/*
Crie uma função que adicione um valor à variável criada acima, e retorne a string:
    O valor da variável agora é VALOR.
Onde VALOR é o novo valor da variável.
*/
function add(value) { semValor = value; return `O valor da variável agora é ${semValor}` };

// Invoque a função criada acima.
add(20);

// Qual o retorno da função? (Use comentários de bloco).
/*
  O valor da variável agora é 20
*/
2
/*
Crie uma função com as seguintes características:
1. A função deve receber 3 argumentos;
2. Se qualquer um dos três argumentos não estiverem preenchidos, a função deve retornar a string:
    Preencha todos os valores corretamente!
3. O retorno da função deve ser a multiplicação dos 3 argumentos, somando `2` ao resultado da multiplicação.
*/
  function multiplique(arg1, arg2, arg3) {
    if (arg1 && arg2 && arg3) {
      return arg1 * arg2 * arg3 + 2;
    } else {
      return 'Preencha todos os valores corretamente';
    }
  }

// Invoque a função criada acima, passando só dois números como argumento.
multiplique(2, 2)

// Qual o resultado da invocação acima? (Use comentários para mostrar o valor retornado).
"Preencha todos os valores corretamente"

// Agora invoque novamente a função criada acima, mas passando todos os três argumentos necessários.
multiplique(2, 2, 2)

// Qual o resultado da invocação acima? (Use comentários para mostrar o valor retornado).
10

/*
Crie uma função com as seguintes características:
1. A função deve receber 3 argumentos.
2. Se somente um argumento for passado, retorne o valor do argumento.
3. Se dois argumentos forem passados, retorne a soma dos dois argumentos.
4. Se todos os argumentos forem passados, retorne a soma do primeiro com o segundo, e o resultado, dividido pelo terceiro.
5. Se nenhum argumento for passado, retorne o valor booleano `false`.
6. E ainda, se nenhuma das condições acima forem atendidas, retorne `null`.
*/
function somando(num1, num2, num3) {
  if (num1 && num2 && num3) return (num1 + num2) / num3
  else if (num1 && num2 && !num3) return num1 + num2
  else if (num1 && !num2 && !num3) return num1
  else if (!num1 && !num2 && !num3) return false
  return null
}

// Invoque a função acima utilizando todas as possibilidades (com nenhum argumento, com um, com dois e com três.) Coloque um comentário de linha ao lado da função com o resultado de cada invocação.
somando(); // false
somando(1); // 1
somando(2, 3); // 5
somando(2, 3, 5) // 1
```
