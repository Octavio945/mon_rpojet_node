Salut à tous,

Préparez-vous, car nous allons plonger dans le monde passionnant de NodeJS ! Ce cours sera axé sur la pratique et la construction d'applications réelles.

Pour commencer, suivez ces étapes pour configurer votre environnement de développement :

Node: 22.15.1

1.  **Créez votre projet :** Ouvrez votre terminal et tapez ces commandes. Cela créera un dossier pour votre projet et initialisera un fichier `package.json` :
    ```bash
    mkdir mon-projet-node  # Crée un dossier pour votre projet
    cd mon-projet-node     # Navigue dans le dossier
    npm init -y           # Initialise le projet avec les paramètres par défaut
    ```
    **Commentaire :** *`npm init -y` crée un fichier `package.json` avec les configurations par défaut.  Ce fichier est crucial pour gérer les dépendances de votre projet.*

2.  **Installez les dépendances:** Installez les bibliothèques dont nous aurons besoin. Ces bibliothèques sont essentielles pour le développement de notre projet :
    ```bash
    # Dépendances de production
    npm install express @prisma/client pg dotenv zod pino pino-http pino-pretty

    # Dépendances de développement
    npm install --save-dev prisma nodemon
    npx prisma init --datasource-provider postgresql
    ```

    **Commentaires :**

    *   `express` : Un framework web pour NodeJS.
    *   `@prisma/client`: Client de base de données.
    *   `pg` : Driver Postgres.
    *   `dotenv` : Pour gérer les variables d'environnement (secrets, etc.).
    *   `zod` : Pour la validation de données.
    *   `pino`, `pino-http`, `pino-pretty`: Pour le logging.
    *   `prisma` : Notre outil pour la gestion de la base de données.
    *   `nodemon` : Pour le rechargement automatique de votre serveur pendant le développement.

3.  **Initialisation de Prisma:** Cette commande va initialiser Prisma dans votre projet et configurer la base de données. Assurez-vous d'avoir PostgreSQL installé et configuré sur votre machine.
    ```bash
    npx prisma init --datasource-provider postgresql
    ```


Nous allons utiliser cette application qui est une alternative à Postman: Yaak
https://yaak.app/


Il faut tout faire pour avoir un dossier avec les packages listés. Si vous rencontrez des problèmes, cherchez. Si vous ne trouvez pas de solution, réfléchissez.