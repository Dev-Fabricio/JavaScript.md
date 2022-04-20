# JavaScript 
<div>
</div>
> Fabrício 10/03/2022
<div>
<br>
<img align="center" alt="Rafa-Js" height="30" width="40" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/javascript/javascript-plain.svg">
<br>
</div>

## Inclusão do javascript - html5 [X]

```javascript
;(<script src="meu_script.js"> </script>)`Utilização de forma externa`
```

`DOM - Document Object Model` é a arvore de documento.

## Comentários [X]

```javascript
//Comentário em uma linha

/*
Comentários em
Multiplas linhas    
*/
```

## Variáveis [X]

Armazena dados. / tipos:

- Strings = Caracteres
- Number = Valores numericos - Int e Float
- Bollean = Armazenamento de estados, TRUE ou FALSE.

Para a declaração das variaveis não se ultiliza `caracteres especiais` ou se inicia com `numeros` além de não utilizar `palavras resevadas da linguagem`

- var / let / const

```javascript
//strings
var texto = 'Curso javascript' // pode usar "" ou ''

//number
var numeroInteiro = -7
var numeroFrancionado = 11210.75

//bollean
var teste = true // true: verdadeiro, false: falso

alert(numeroFrancionado) // Abrir um dialog
document.write(texto) // Inseção de texto
prompt() // Opção de digitar algo.
console.log() // Gera um log no console
```

## Concatenação [X]

```javascript
var nome = prompt('Digite seu nome:')
var idade = prompt('Digite seu nome:')
document.write(<h1>  Bom dia ' + nome + ', você tem ' + idade + ' anos.<h1>)
```

## Utilização do `;` [X]

Não é obrigatório poŕem não causa `erro` usar.

## Variáveis Null e Underfined [X]

```javascript
//Null
var teste = null //Ausencia de um valor

//Unndefined
var teste2 //Variável vazia.
```

## Alteração dos valores das variáveis [X]

- As variáveis podem ser alteradas, ex:

```javascript
var teste = 'Augusto'
console.log(teste) //R: Augusto
teste = 'Fabrício'
console.log(teste) //R: Fabrício
```

## If / Else [X]

```javascript
//If = se
//Else = senão

if (condição) {
  //trecho de código que será executada.
} else {
  //trecho de código que será executada.
}

/* 
    Outra alternativa / caso o a condição do if não esteja correta, tentaremos a condição do else if.
    */

if (condição) {
  //trecho de codigo que será executada.
} else if (condição) {
  //trecho de codigo que será executada.
} else {
  //trecho de codigo que será executada.
}
```

## Operadores de Comparação [X]

- Igual (==) : Verifica se os valores comparados são `iguais`.
- Idêntico (===) : Verifica se os valores comparados são `iguais e do mesmo tipo.`
- diferente (!=) : Verifica se os valores comparados são `diferentes`.
- Não indêntico (!==) : Verifica se os valores comparados `são diferentes e de tipos distintos`.
- Menor (<) : Verifica se o valor da esquerda e `menor` que o da direita.
- Maior (>) : Verifica se o valor da esquerda e `maior` que o da direita.
- Menor igual (<=): Verifica se o valor da esquerda e `menor ou igual` ao da direita
- Maior igual (>=) Verifica se o valor da esquerda e `maior ou igual` que o da direita

## Casting de tipos [X]

```javascript
var v1 = prompt('digite um numero:') //exemplo 2
var v2 = prompt('digite outro numero: ') //exemplo 5

documento.write(v1 + v2)
/* O Resultado será 25, pois a atribuição do prompt é uma string */

v1 = parseInt(v1) -> Transforma String em Number
v2 = parseInt(v2)

document.write(v1 + v2) //Resultado 7

parseFloat() //-> Preserva a fração de um número, ex: 12.50

document.write(v1.toString() + v2.toString())
// Irá contatenar o v1 e o v2.

```

## Operadores Logicos [X]

Operadores que nos permitem conectar operações de comparação `(true e false)`

- E ( && ) : Verdadeiro se `todas` as expressões forem `verdadeiros`.

- OU ( || ) : Verdadeiro se `uma das` expressões forem `verdadeira`.

- Negação ( ! ) : `Inverte` o resultado da expressão de comparação.

## Operadores Ternários [X]

```javascript
var resultado =
  nota >= media && faltas <= faltas_maximas ? 'Aprovado' : 'Reprovado'

document.Write(resultado)
//resultado será calculado pelos operadores térnarios acima.

/*
A utilização dos operadores ternários é igual ao do if else.
*/
```

## Switch [x]

De certa forma é igual ao if / else, porém escrita de forma diferente.

```javascript
var opcao = 2
switch (opcao /*  Pode ser utilizado qualquer tipo de parametro  */) {
  case 1:
    //trecho de código a ser exibido
    break
  case 2:
    //trecho de código a ser exibido
    break
  case 3:
    //trecho de código a ser exibido
    break
  case 4:
    //trecho de código a ser exibido
    break
  default:
    //trecho de código a ser exibido
    break /***  - Break não obrigatório no default -  ***/
}
```

## Operadores Aritimeticos [x]

Utilizados para fórmulas `Mátematicas` nos scripts.

- Adição ( + ) : Soma valores,
- Subtração ( - ) : Diferença entre valores.
- Multiplicação ( \* ) : Produto do valores.
- Divisão ( / ) : Quociente dos valores.
- Módulo ( % ) : Resto existente de uma operação de divisão.
- Incremento ( ++ ) : Pré/pós incremento - `ex: v= 10, v++ / v=11`
- Decremento ( -- ) : Pré/pós descremento - `ex: v= 10, v-- / v=9`

```javascript
var a = 5
var b = 2

documente.write('a soma entre a e b é: ' + (a + b))
//Vai voltar o resultado depois da execução do código.

var teste = 10
var teste2 = 10
teste = teste + 5 -> // Será 15
teste2 += 5 // Será 15 - Forma simplificada.

/****  Pode ser ultilizado em todas as operações aritimeticas  ****/

//
var name = Jorge
name += ', Bom dia'
console.log('name') // -> Resultado: Jorge, Bom dia
```

## Precendencia dos operadores aritimeticos [X]

- `( )` Aplica a precendência  
   1- Multiplicação e Divisão.  
   2- Soma e subtração.

## funções [X]

Encapsular um bloco com um
objetivo definido

```javascript
function calcularAreaTerreno(
  largura,
  comprimento /***Paramentros / variaveis ***/
) {
  var area = largura * comprimento
  return area
}
```

- Existe 2 tipos de funções: as que geram alguma lógica (void) ou a que gera lógica e retorna algum valor.

`exemplo:`

```javascript
function calcularAreaTerreno(largura, comprimento) {
  //lógica
  var area = lagura * comprimento
  document.write('O terreno possui ' + area + ' Metros de quadrados')
}

calcularAreaTerreno(15, 25)

// ================================

function calculAreaTerreno(largura, comprimento) {
  var area = comprimento * largura
  return area
}

var largura = prompt('Digite a largura do terreno (Metros):')

var comprimento = prompt('Digite o comprimento do terreno (Metros):')

var area = calcularAreaTerreno(largura, comprimento)
```

## Escopo de variáveis [X]

- Existem 3 Escopo no JS

1. Global --> `Todo o script`
2. Função --> `Escopo que funciona dentro das funções`
3. Bloco --> `Contidas dentro de chaves no if,else if,switch.`

- **Escopos de funções e de blocos visualizão os globais, porém globais não visualizão os de funções.**

## Funções anonimas / Tecnica de Wrapper [X]

- Não possui nome;

```javascript
var exibirSaudacao = function (nome) {
  documento.write('Olá' + nome + ', tudo bem?')
}

exibirSaudacao('Jorge')
// Visualização na wEB: Olá Jorge, tudo bem?
```

## Funções de Callback [X]

- Funções encaminhadas como parametro para outras funções.

```javascript
function exibirArtigo(id, callbackSucesso, CallbackErro) {
  //Lógica - Recuperaro id via requisição http
  if (true) {
    callbackSucesso(
      'Funções de Callback em JS',
      'Funções de callback são interresantes'
    )
  } else {
    callbackErro('Erro ao recuperar dados.')
  }
}

var callbackSecesso = function (titulo, descricao) {
  document.write('<h1>' + titulo + '</h1>')
  document.write('</hr>')
  document.write('<p>' + descricao + '</p>')
}
var callbackErro = function (erro) {
  document.write('<p>Erro: ' + erro + '</p>')
}

exibirArtigo(1, callbackSucesso, callbackErro)
```

## Funções para manipular Strings [Z]

- ex: `document.write('Fabricio'.length)`
  --> o Retorno será a quantidade de letras contida na String. `[Atributo Length]`.

- Alguns das funções contém índice - ex:  
  `document.write('Fabricio'.charAt(3))` --> O B que é a 3ª palavras será a resposta a ser dada pelo write.
- O `index.of()` é o inverso do `charAt()`.

* https://www.w3schools.com/jsref/jsref_obj_string.asp

## Funções nativas para tarefas Mátematicas [Z]

```javascript
var x = Math.ceil(10.35)
// --> Irá força o valor a ser "arredondando" para cima, nesse exemplo será 11.

var y = Math.floor(10.6)
// --> Irá força o valor a ser "arredondando" para baixo, nesse exemplo será 10.

var z = Math.round(10.6)
// --> Irá "arredondar" para o lugar mais proximo, ex: 600 para cima, 400 para baixo.

Mah.random() //--> Valores aleatórios entre 0 - 1.
```

## Funções nativas para manipulação de Data. [Z]

```javascript
var date = new Date()
document.write(data.getDate() + '/' + (data.getMonth() + 1) + '/' date.getFullYear())



// --> o getMonth considera o inicio do ano (janeiro) como 0 e vai subindo sucessivamente.


// --> o metodo get é para recuperar dados, o set é para atribuir um dado.


var date = new Date()
document.write(data.toString())
// Resultado: Fri Mar 11 2022 08:27:28 GMT-0300 (Horário Padrão de Brasília)
data.setDate(data.getDate() + 1)
document.write(data.toString())
// Irá retornar o dia atual + 1, exemplo dia 11 irá ser dia 12.
// --> o set mudará não só o dia, mas também mês e anos, até mesmo no setDate
```

## Eventos [Z]

### mouse:

- onlick `-->` quando a click do mouse
- ondblclick `-->` quando a 2 clicks sequenciais
- onmouseup `-->` quando solta o click
- onmouseover `-->` quando colocar o mouse
- onmouseout `-->` quando retira o mouse

### teclado:

- onkeydown `-->` Quando uma tecla é presionada
- onkeypress `-->` Quando mantém a tecla pressionada (porém apenas nos que soltam caracteres)
- onkeyup `-->` quando a tecla e soltada

### Janela:

- onresize `-->` Quando a janela for redimencionada
- onscroll `-->` Quando o scroll for utilizada

### Formulários

- onfocus `-->` quando recebe o foco do curso do mouse
- onblur `-->` quando perde o foco do mouse
- onchanger `-->` quando sofre uma modificação

## DOM [Z]

- Document Object Model / API que permite o acesso via JavaScript aos elementos da página.

![Arvore DOM](https://miro.medium.com/max/1200/1*mMmuOhNytgqP7lrU9HPTpw.jpeg)

### document (API Dom)

- Seleção de elementos do HTML

```javascript
getElementById() // Id
getElementsByTagName() // TagName
getElementsByClassName() // Class
getElementsByName() // Name
```

### Manipulação

- atributo style --> modifica estilo no js
- Existe diverso, esse só um `exemplo`.

```javascript
//   ***** EXEMPLO ******
funtion modificarClasse() {
    document.getElementById('botton1').className = 'estilo2'
}
```

## Array Básico [X]
* basicamente, são listas!, são variaveis que nós permitem relacionar itens a indices ou chaves.

~~~javascript
// --> Com variáveis (não recomendado):
var fruta1 = 'maça'
var fruta2 = 'banana'
var fruta3 = 'abacate'
var fruta4 = 'goiaba'


// --> Com um único array:
var fruta = Array();
fruta[1] = 'maça'
fruta[2] = 'banana'
fruta[3] = 'abacate'
fruta[4] = 'goiaba'
/* 
    Também pode ser utilizado Strings para denominar os Arrays
    ex: `fruta['x'] = 'maça'` 
    OU mudanças de Valores 
    ex: `fruta['y'] = true, fruta[100] = 200`

    =====

    var fruta = Array()
          OU
    var fruta = []
    O javascript tem capacidade de indentificar que o [] é um Array.
*/

var fruta = Array('Banana', 'Maçã', 'Goiaba', 'abacate')
var fruta = ['Banana', 'Maçã', 'Goiaba', 'abacate']
// --> Essa também é uma forma de declara um Array e seus componetes, assim será declarado de forma númerica começando pelo 0, ex: Banana --> 0;
~~~

* O `.legth` na `string` retorna a quatidade de `carácteres`, já nos `Arrays( )` retona a quantidade de `elementos`. A diversas regras para o .legth retornar a quantidade de elementos no Array: ter todos os indices numeros sem pulos, começando pelo 0. 

## Array Multidimensionais [X]
* são arrays de arrays
~~~javascript
var lista_coisas = []  

lista_coisas['frutas'] = Array('Banana', 'Maçã', 'Goiaba', 'Uva') 
listas_coisas['pessoas'] = ['João', 'José', 'Maria']

document.write(listas_coisas['frutas'][3])
// --> O resultado será = Uva.
~~~

## Adicionar / Remover Elementos dos Arrays [X]
~~~javascript
var lista_frutas = ['Banana', 'Maçã']


/*  ================      Adicionar      ==================        */
lista_frutas.push('Uva') // Resultado 0= Banana, 1= Maçã, 2= Uva.
lista_frutas.unshift('Uva') // // Resultado 0= Uva, 1= Banana, 2= Maçã.



/*  ================      Exluir         =================       */
lista_frutas.pop() // Elemento do final do Array
lista_frutas.shift() // Elemento do inicio do Array

~~~

## Arrays, Método de pesquisa: [X]
~~~javascript
var lista_frutas = ['Banana', 'Maçã', 'Morango', 'Uva']

console.log(lista_frutas.indexOf('Morango'))
 // --> Retorno do index numerico ou alfanumerico, se não existe o elemento vai ser retornado -1.

/*   OBS: As letras devem ser igual a escrita em relação a letras maiscula e minusculas.    */
~~~

## Ordenação de elementos Arrays [X]

~~~javascript 
var lista_frutas = ['Maçã', 'Uva', 'Banana', 'Morango']
Console.log(listas_frutas.sort()) // Ordenação Alfanumérica, ordem alfabética

/*==================*/
var lista_numeros = [3, 9, 10, 2, 5]
Console.log(lista_numeros.sort(ordenaNumeros)) // Sem parametros na function do sort.

funtion ordenaNumeros(a, b) {
  return a - b
}

~~~




