# Binary Patching

## 1. Etudier le binaire

Dans un premier temps il faut étudier le binaire afin de savoir ce qu'il fait. Pour se faire on peut l'exécuter, puis le décompiler à l'aide de :
```
objdump -d program
``` 
Ensuite on va parcourir l'assembleur que l'on vient de décompiler à l'aide de `objdump`. On va chercher la portion qui nous interesse et que l'on veut modifier.

## 2. Modification du binaire
Une fois la portion de binaire que l'on veut modifier trouvée, on va utiliser la commande :
```
printf '\x??' | dd of=program bs=1 seek=? count=? conv=notrunc
```
Avec printf qui correspond à la nouvelle valeur de ce qu'on veut modifier, seek qui correspond à sa position dans le binaire, count le nombre de bytes à modifier.

## 3. Alternative
On peut combiner les deux étapes avec `ghidra` qui va nous permettre de décompiler directement le binaire et d'avoir la corrélation entre le binaire et l'assembleur décompiler. Puis on peut cliquer sur une portion du binaire pour le modifier. Ensuite on exporte le nouveau binaire créé puis il ne reste plus qu'a le compiler.


