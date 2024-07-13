# ROCKNITE-MUSIQUE

**ROCKNITE-MUSIQUE** est un site web innovant qui vous permet d'écouter votre musique locale à distance, sans publicité.

## Fonctionnalités

- **Streaming sans publicité** : Profitez de votre musique locale sans interruptions publicitaires.
- **Bibliothèque musicale personnelle** (en développement) : Accédez à votre propre collection de morceaux et albums.
- **Playlists personnalisées** (en développement) : Créez et organisez vos propres playlists selon vos goûts musicaux.
- **Synchronisation multi-appareils** : Écoutez votre musique sur plusieurs appareils sans perdre vos préférences.
- **Qualité audio optimale** : Profitez d'un son haute définition pour une expérience d'écoute exceptionnelle.

## Installation

Pour utiliser ce projet, suivez ces étapes :

1. **Téléchargement et décompression** :
    - Téléchargez le fichier ZIP du projet depuis le dépôt GitHub.
    - Décompressez le fichier ZIP téléchargé.

2. **Configuration** :
    - Accédez au répertoire décompressé.
    - Naviguez vers le dossier `search`.
    - Ouvrez le fichier `musique.json` avec un éditeur de texte.
    - Ajoutez les informations de vos fichiers musicaux dans `musique.json`.

3. **Ajout de fichiers musicaux** :
    - Placez vos fichiers musicaux dans le dossier `search/musique`.

## Utilisation

Vous avez deux options pour utiliser le site web :

### Utilisation locale

1. Ouvrez le fichier `index.html` dans votre navigateur pour lancer le site web en local.

### Utilisation en ligne

Vous pouvez également héberger le site en ligne en utilisant Python 3 et Serveo avec AutoSSH, ou Ngrok.

#### Avec Python 3 et Serveo

1. Installez Python 3 si ce n'est pas déjà fait.
2. Ouvrez un terminal et naviguez vers le répertoire du projet.
3. Lancez un serveur HTTP avec la commande suivante :

    ```bash
    # Lancer un serveur HTTP local
    $ python3 -m http.server
    ```

4. Utilisez Serveo et AutoSSH pour rendre le serveur accessible en ligne :

    ```bash
    # Utiliser Serveo pour rendre le serveur accessible en ligne
    $ ssh -R 80:localhost:8000 serveo.net
    ```

#### Avec Ngrok

1. Installez Ngrok depuis [ngrok.com](https://ngrok.com).
2. Ouvrez un terminal et naviguez vers le répertoire du projet.
3. Lancez un serveur HTTP avec Python 3 :

    ```bash
    # Lancer un serveur HTTP local
    $ python3 -m http.server
    ```

4. Lancez Ngrok pour rendre le serveur accessible en ligne :

    ```bash
    # Utiliser Ngrok pour rendre le serveur accessible en ligne
    $ ngrok http 8000
    ```

Ngrok vous fournira une URL publique que vous pourrez utiliser pour accéder à votre site web.

## Faire un Don
Si vous aimez ce projet et souhaitez soutenir son développement, vous pouvez faire un don via [Patreon](patreon.com/ROCKNITE_MUSIQUE). Votre soutien est grandement apprécié et nous aide à continuer à améliorer ROCKNITE-MUSIQUE.

## Licence

Ce projet est sous licence MIT - voir le fichier [LICENSE](LICENSE) pour plus de détails.
