# Simple description de mon header filou et de ses effets :
J'ai fait un simple header en C où les fonction portant le nom de chat font un *printf* avec une phrase ou une référence (que je trouve) rigolote. Pour l'instant j'ai quatres noms de chat dedans mais y'a des chances que j'en rajoutte par la suite :
1. Filou
2. Echo
3. Guppy
4. Zenit

Voici le header :
```C
#ifndef FILOU_H
#define FILOU_H

#include <stdio.h>

#define filou printf("Miaou\n")
#define echo7 printf("MAOW\n")
#define guppy printf("Louez soit le saint Guppy!\n")
#define zenit printf("Zenit\n")

#endif
```
Voilà donc c'est simplement un test à la con pour voir comment peux fonctionner un header en C (mais j'imagine qu'en C++ ça doit être la même chose ou du moin assez proche). Et par conséquant dans le fichier en .c ça donne :
```C
#include "filou.h"

int main(void)
    {
        filou;/*Should display Miaou*/
        echo7;/*Should display MAOW*/
        guppy;/*Shoudl display Louez soit le saint Guppy!*/
        zenit;/*Should display Zenit*/

        return 0;
    }
```
