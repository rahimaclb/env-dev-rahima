# Fiche réseau 
 
## Mes adresses IP 
 
| Machine                | Adresse IP     | Privée ou publique ? | 
| ---------------------- | -------------- | -------------------- | 
| Mon Ubuntu             | 172.28.171.222 | Privée               | 
| Mon ordinateur (Wi-Fi) | 172.16.50.245  | Privée               | 
| Ma connexion Internet  | (non publiée)  | publique             | 
 
## Résultats du DNS 
 
| Nom de domaine  | Adresse IP   | 
| --------------- | ------------ | 
| `github.com`    | 140.82.121.3 | 
| `wikipedia.org` | 185.15.59.224| 
 
## Les outils réseau 
 
| Commande             | Ce qu'elle fait                                                             | 
| -------------------- | --------------------------------------------------------------------------- | 
| `hostname -I`        | Affiche l'adresse IP de mon Ubuntu                                          | 
| `ping -c 4 <nom>`    | Envoie 4 paquets à la machine indiquée pour vérifier si elle est joignable. |                                            | 
| `nslookup <nom>`     | Recherche l’adresse IP associée au nom de domaine indiqué.                  |

## Le trajet d'une requête

Quand je tape `https://github.com` dans mon navigateur :

1. Le navigateur extrait le nom de domaine `github.com` de l’adresse.
2. Le DNS recherche l’adresse IP associée à ce nom de domaine.
3. L’ordinateur envoie une requête vers cette adresse IP en passant par le réseau et le routeur.
4. Le serveur de GitHub reçoit la requête et renvoie une réponse.
5. Le navigateur reçoit la réponse et affiche la page.
6. La communication HTTPS chiffre les données échangées entre le navigateur et le serveur.

## Les codes de réponse HTTP

| Code | Nom                   | Ce qu'il veut dire                                                                        | Exemple que j'ai vu                                                |
| ---- | --------------------- | ----------------------------------------------------------------------------------------- | ------------------------------------------------------------------ |
| 200  | OK                    | La requête a réussi et le serveur a renvoyé le contenu demandé.                           | La page d’accueil de GitHub s’affiche correctement.                |
| 301  | Moved Permanently     | La page a été déplacée définitivement vers une autre adresse. Le navigateur est redirigé. | Une ancienne adresse redirige vers la nouvelle adresse de la page. |
| 404  | Not Found             | Le serveur ne trouve pas la page ou la ressource demandée.                                | Une page inexistante ou une URL mal écrite.                        |
| 500  | Internal Server Error | Une erreur interne empêche le serveur de traiter la requête.                              | Pas vu.                                                            |