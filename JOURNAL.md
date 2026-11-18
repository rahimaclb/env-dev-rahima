# Journal des choix

## 2026-11-11 -installation de tree
 
 - **Décision :** installer Node.js avec le gestionnaire de paquets `apt` en mode adminstrateur avec `sudo` .
 - **Autres possibilités :** le paquet nodejs d'Ubuntu, le site nodejs.org.
 - **Raison :** NodeSource donne la version LTS récente, et les commandes peuvent être écrites dans mon README pour être refaites à l'identique. 

 ## 2026-11-03 – Système pour le terminal 

 - **Décision :** utiliser Ubuntu 24.04 dans WSL sur mon PC Windows.
 - **Autres possibilités :** installer une machine irtuelle avec VirtualBox, faire un dual-boot Ubuntu, ou utiliser Git Bash 
 - **Raison :** WSL s'ouvre directement sans ralentire l'ordinateur, donne un  vrai terminal Ubuntu Identique à celui d'un serveur et fonctionne directemet avec VS code avec VS Code.

 ## 2026-11-05 – Éditeur de code

- **Décision :** utiliser VS Code avec l'extension WSL.
- **Autres possibilités :** Notepad++, Sublime Text, ou éditer seulement dans le terminal avec nano.
- **Raison :** VS Code permet d'ouvrir le dossier du projet depuis Ubuntu avec la commande `code .`, d'avoir le terminal intégré en bas et de voir le rendu Markdown avec Ctrl + Maj + V.

## 2026-11-12 – Version de Node.js : LTS

- **Décision :** installer la version LTS (v22.x) de Node.js avec un numéro majeur pair.
- **Autres possibilités :** installer la dernière version impaire (Current, comme la v23).
- **Raison :** les versions LTS sont stables et maintenues pendant 3 ans. Cela évite que les programmes plantent avec des erreurs d'incompatibilité quand on partage son projet avec un camarade.

## 2026-11-17 – Installation de Node.js

- **Décision :** installer Node.js avec le dépôt NodeSource et apt.
- **Autres possibilités :** le paquet nodejs d'Ubuntu, le site nodejs.org.
- **Raison :** NodeSource donne la version LTS récente, et les commandes peuvent être écrites dans mon README pour être refaites à l'identique.

## 2026-11-19 – Scripts d'installation et de vérification

- **Décision :** écrire deux scripts Bash `scripts/installer.sh` et `scripts/verifier.sh`.
- **Autres possibilités :** retaper toutes les commandes à la main à chaque fois ou les copier-coller une par une depuis le README.
- **Raison :** avec un script, on ne fait pas de faute de frappe, on installe tout en une seule commande et mon binôme peut vérifier tout de suite si son poste est prêt.
