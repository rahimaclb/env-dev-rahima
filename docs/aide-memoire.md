# Aide-mémoire du terminal Linux

## Se déplacer

| Commande | Ce qu'elle fait               | Exemple    |
| -------- | ----------------------------- | ---------- |
| `pwd`    | Affiche le dossier où je suis | `pwd`      |
| `cd`     | Change de dossier             | `cd ~/dev` |
| `cd ..`  | Remonte d'un dossier          | `cd ..`    |
| `ls`     | Liste le contenu du dossier   | `ls -la`   |
| `clear`  | Efface l'écran du terminal    | `clear`    |

## Fichiers et dossiers

| Commande | Ce qu'elle fait                    | Exemple                 |
| -------- | ---------------------------------- | ----------------------- |
| `mkdir`  | Crée un dossier                    | `mkdir docs`            |
| `touch`  | Crée un fichier vide               | `touch notes.txt`       |
| `cp`     | Copie un fichier                   | `cp a.txt b.txt`        |
| `cp -r`  | Copie un dossier et son contenu    | `cp -r docs docs_copie` |
| `mv`     | Déplace ou renomme un fichier      | `mv a.txt docs/`        |
| `rm`     | Supprime un fichier                | `rm b.txt`              |
| `rm -r`  | Supprime un dossier et son contenu | `rm -r docs_copie`      |
| `rmdir`  | Supprime un dossier vide           | `rmdir vide`            |

## Lire et chercher

| Commande | Ce qu'elle fait                   | Exemple                   |
| -------- | --------------------------------- | ------------------------- |
| `cat`    | Affiche le contenu d'un fichier   | `cat notes.txt`           |
| `less`   | Lit un fichier page par page      | `less notes.txt`          |
| `head`   | Affiche les premières lignes      | `head -n 5 notes.txt`     |
| `tail`   | Affiche les dernières lignes      | `tail -n 5 notes.txt`     |
| `grep`   | Cherche un mot dans un fichier    | `grep "erreur" notes.txt` |
| `find`   | Cherche un fichier par son nom    | `find . -name "*.md"`     |
| `wc`     | Compte lignes, mots et caractères | `wc -l notes.txt`         |
| `echo`   | Affiche du texte                  | `echo "Bonjour"`          |

## Aide et astuces

| Commande  | Ce qu'elle fait                  | Exemple   |
| --------- | -------------------------------- | --------- |
| `man`     | Affiche le manuel d'une commande | `man ls`  |
| `history` | Montre les commandes déjà tapées | `history` |
| `whoami`  | Affiche mon nom d'utilisateur    | `whoami`  |

## Branches Git

| Commande        | Ce qu’elle fait                                   | Exemple          |
| --------------- | ------------------------------------------------- | ---------------- |
| `git branch`    | Affiche les branches et indique la branche active | `git branch`     |
| `git switch`    | Change de branche                                 | `git switch main` |
| `git switch -c` | Crée une branche et bascule dessus                | `git switch -c ma-branche` |
| `git merge`     | Fusionne une branche dans la branche active       | `git merge ma-branche`     |
| `git log --oneline --graph --all` | Affiche l’historique de toutes les branches | `git log --oneline --graph --all` |
| `git push`      | Envoie les commits vers le dépôt distant          | `git push` |
| `git branch -d` | Supprime une branche déjà fusionnée               | `git branch -d ma-branche` |

## Astuce de Lisa
 
`git log --oneline --graph` dessine l'historique avec les branches.