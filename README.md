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
:set promp ">"
```
t
