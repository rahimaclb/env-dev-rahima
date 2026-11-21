# Journal des choix

## 2026-11-03 – Système pour le terminal

- **Décision :** utiliser Ubuntu 26.04.1 dans WSL sur mon PC Windows 11.
- **Autres possibilités :** installer une machine virtuelle avec VirtualBox, installer Ubuntu en double démarrage ou utiliser Git Bash.
- **Raison :** WSL permet d’utiliser un terminal Ubuntu directement depuis Windows, sans démarrer une machine virtuelle séparément. Ce terminal est adapté au travail sur des projets et fonctionne avec VS Code.

## 2026-11-05 – Éditeur de code

- **Décision :** utiliser VS Code avec l’extension WSL.
- **Autres possibilités :** utiliser Notepad++, Sublime Text ou éditer les fichiers uniquement dans le terminal avec nano.
- **Raison :** VS Code permet d’ouvrir le dossier du projet depuis Ubuntu avec la commande `code .`. Il comprend un terminal intégré et permet de prévisualiser les fichiers Markdown avec `Ctrl` + `Maj` + `V`.

## 2026-11-11 – Installation de tree

- **Décision :** installer `tree` dans Ubuntu avec la commande `sudo apt install -y tree`.
- **Autres possibilités :** utiliser la commande `ls` pour afficher le contenu des dossiers ou parcourir les dossiers un par un.
- **Raison :** `tree` affiche les dossiers et les fichiers sous forme d’arborescence. Cela permet de voir plus facilement l’organisation du projet dans le terminal.

## 2026-11-12 – Version de Node.js : LTS

- **Décision :** utiliser Node.js 26.x, la version indiquée dans mon README.
- **Autres possibilités :** utiliser une autre version de Node.js proposée par Ubuntu ou une version Current.
- **Raison :** je veux utiliser une version adaptée à mon environnement et garder une version cohérente entre mon installation et la vérification des logiciels.

## 2026-11-17 – Installation de Node.js

- **Décision :** installer Node.js avec le dépôt NodeSource et `apt`.
- **Autres possibilités :** installer le paquet `nodejs` d’Ubuntu ou télécharger Node.js depuis [nodejs.org](https://nodejs.org).
- **Raison :** cette méthode permet d’installer Node.js avec les outils de gestion de paquets utilisés dans Ubuntu. Les commandes d’installation peuvent être indiquées dans le README pour être retrouvées et réutilisées.

## 2026-11-19 – Scripts d’installation et de vérification

- **Décision :** écrire deux scripts Bash, `scripts/installer.sh` et `scripts/verifier.sh`.
- **Autres possibilités :** retaper les commandes à la main ou les copier-coller une par une depuis le README.
- **Raison :** les scripts regroupent les commandes d’installation et de vérification. Ils réduisent les risques de faute de frappe et permettent à mon binôme de vérifier rapidement si son poste est prêt.