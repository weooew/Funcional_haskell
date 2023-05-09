# Funcional_haskell

## Haskell(functional language) features:
* functions with no side effects (can't set a variable to one value then change it)
* referential transparency (if called by same parameters ALWAYS return same resullt)
* lazy (only execute funcions when it needs to show the result, cause no matter when you calcule it will have the same result; allows infinite results)

```
xs = [1,2,3,4,5,6,7,8]
DoubleMe(DoubleMe(DoubleMe(xs)))
--this code in imperial language: 3 times->pass through,do copy,return it
--in haskell: only one time (cause is lazy)
````
* Statically typed (compiler identifies whats a string, whats an int...)

Gettin Started---------------------------------------------------------
```
--how to instal ghci in terminal of linux:
sudo apt install haskell-plataform
--how to open ghci in terminal
ghci
--how to set promp
:set promp "prelude>"
```

Calculadora do haskell
```
2**3 -->8
2^3 -->8
-1^2 -->1
1/0 -->Infinity
```
Obs: diferente é '\='

Importar arquivo (l significa load) in ghci
```
:l nomearq
```

Prefix Functions
```
odd x
even x
succ 10 -->11
min 3 4 -->3
max 3 4 -->4
--if it takes 2 parameters can become infix function (witch can be easier to read)
div 92 10 --or: 92 'div' 10 -- >9
mod x y --or: x 'mod' y
--can't mod x [1,2]
```
Doing Funcions
```
doubleMe x = x+x
doubleUs x y = x*2+y*2
doubleUs x y = doubleMe x + doubleMe y 

doubleSmall x = if x > 100 then x else x*2 --else is mandatory, every has to return something
--OBS: variables can't begin with capital letter; but can use underline ' in there names. Exemple:
conor_O'Brien = "hello"
```
Lists
```
-- TEXAS RANGERS
list1 = [1..10] --vai aumentando de um em um
--[1,2,3,4,5,6,7,8,9,10]

list2 = [1.0,1.5..3.0]  --vai aumentando de x em x (x = elem2-elem1)
--[1.0,1.5,2.0,2.5,3.0]

list3 = [10,9..0] --vai diminuindo de acordo com o valor do intervalo dos primeiros elementos
--[10,9,8,7,6,5,4,3,2,1,0] ps: can only specify a sigle step (so kind of ambiguous)
--wrong: nameOFlist = [10..0] cause it would want to put +1 that way impossible to reach 0

multiplos_de_13 = [13, 26.. 24*13] == take 24[13,26..] --os 24 primeiros multiplos de 13

smallCaseAlf = ['a'..'z']

-- CONCATENATION
[1,2,3] ++ [4,5] -- > [1,2,3,4,5]
--wrong: [1,2,3] ++ 4
[1,2,3] ++ [4] -- > [1,2,3,4]

"hello" ++ " world" -->hello world
['w','h'] ++ ['a','t'] -->what

5:[1,2,3] -->[5,1,2,3]
5:3:[1] -->[5,3,1]
'A'++ "SMALL CAT" --> A SMALL CAT

-- INDEX (!!)
"Steve Jobs" !! 6 --> B
[9.2,12.1,3.7] !! 1 --> 12.1

-- COMPARING LISTS

-- MORE LIST FUNCTIONS

```




```
--:t para verificar o tipo da variável ou função
:t s
```

