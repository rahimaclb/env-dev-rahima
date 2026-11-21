# env-dev-rahima (B1 DEV, IFRAN) – Mon environnement de développement

Environnement de développement de Rahima COULIBALY – B1 DEV, IFRAN.

## Mon ordinateur

| Élément     | Valeur                    |
| ----------- | -------------------       |
| Système     | Windows 11 Professionnel  |
| Processeur  | Intel Core i7             |
| Mémoire     | 16 Go                     |
| Éditeur     | VS Code                   |

## Mon Ubuntu

| Élément      | Valeur                   |
| ------------ | --------------------     |
| Version      | Ubuntu 26.04.1 LTS       |
| Lancé avec   | WSL                      |
| Processeurs  | 12                       |
| Mémoire      | 7,6 Go                   |
| Utilisateur  | rahima                   | 

## Logiciels installés dans Ubuntu

| Logiciel | Version | Commande d'installation                             |
| -------- | ------- | --------------------------------------------------- |
| Git      | 2.43.0  | déjà présent dans Ubuntu                            |
| tree     | 2.1.1   | `sudo apt install -y tree`                          |
| htop     | 3.3.0   | `sudo apt install -y htop`                          |
| nano     | 7.2     | `sudo apt install -y nano`                          |
| Node.js  | 26.xx   | dépôt NodeSource, puis `sudo apt install -y nodejs` |
| npm      | 11.xx   | installé avec Node.js                               |

## Installation

### 1. Installer Ubuntu sous WSL sur Windows 11 et VS Code

- Dans le Terminal Windows ouvert en tant qu’administrateur, taper `wsl --install`, puis redémarrer l’ordinateur.
- Au premier lancement d’Ubuntu, choisir un nom d’utilisateur et un mot de passe.
- Installer VS Code depuis [code.visualstudio.com](https://code.visualstudio.com).

### Sur Mac

- Installer Homebrew depuis [brew.sh](https://brew.sh).
- Dans le Terminal, taper `brew install colima docker`.
- Démarrer Colima avec `colima start`, puis se connecter avec `colima ssh`.
- Installer VS Code depuis [code.visualstudio.com](https://code.visualstudio.com).

### 2. Installer les outils dans Ubuntu

1. Ouvrir Ubuntu et aller dans le dossier du projet : `cd ~/dev/env-dev-rahima`
2. Lancer le script d’installation : `./scripts/installer.sh`

## Vérification

Lancer `./scripts/verifier.sh` dans Ubuntu.

Résultat attendu : une version pour Ubuntu, Git, Node.js, npm et `tree`.


## Contenu du dossier

| Fichier ou dossier     | Rôle                                                         |
| ---------------------- | ------------------------------------------------------------ |
| `README.md`            | Cette documentation                                          |
| `JOURNAL.md`           | Le journal de mes choix                                      |
|`docs/aide-reseau.md`   | Ma fiche de reseau                                           |                 
| `docs/aide-memoire.md` | Mon aide-mémoire des commandes du terminal Linux             |
| `scripts/installer.sh` | Script qui installe les outils (Git, Node.js, npm, tree…)    |
| `scripts/verifier.sh`  | Script qui affiche les versions pour vérifier l'installation |