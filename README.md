# *Funções de Alta Ordem*
Em Haskell, uma função de alta ordem é uma função que recebe outra função como argumento, ou retorna uma função como resultado.
Isso é possível porque em Haskell funções são valores, podendo ser passadas, armazenadas em variáveis e reutilizadas durante o código.

# *Função Lambda*
Uma função lambda é uma função anônima, ou seja, uma função sem nome, usada geralmente em situações simples e temporárias.

Em Haskell, lambdas são escritas usando \.

# *Exemplo de funções em Haskell*
Any e All (Verificação Lógica)
Estas funções recebem um predicado (uma função que retorna verdadeiro ou falso) e uma lista.

All: Retorna True apenas se todos os elementos satisfizerem a condição.

Any: Retorna True se pelo menos um elemento satisfizer a condição.
```Haskell
notas = [8, 9, 7, 10, 5]

-- Todos passaram (nota >= 7)?
todosPassaram = all (>= 7) notas
-- Resultado: False (por causa do 5)

-- Alguém tirou nota máxima (10)?
alguemGabaritou = any (== 10) notas
-- Resultado: True
```

# Exemplos dessas funções em Javascript
No JS, os equivalentes para all e any são os métodos .every() e .some().
```Javascript
const notas = [8, 9, 7, 10, 5];

// Todos passaram (nota >= 7)?
const todosPassaram = notas.every(n => n >= 7);
// Resultado: false

// Alguém tirou nota máxima (10)?
const alguemGabaritou = notas.some(n => n === 10);
// Resultado: true
```

Também temos a função zipWith (Combinação de Listas) na linguagem Haskell. Ela une duas listas elemento por elemento usando uma função de combinação que você define.
```Haskell
listaA = [1, 2, 3]
listaB = [10, 20, 30]

-- Multiplica os elementos de A pelos de B na mesma posição
resultado = zipWith (*) listaA listaB
-- Resultado: [10, 40, 90]
```


