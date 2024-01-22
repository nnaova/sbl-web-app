# SBL-web-app

Application à destination de la Splatoon Baguette League, qui organise des tournois sur le jeu Splatoon 3. L'application permettra de gérer la ligue organisé par la SBL, ainsi que les tournois qui y seront organisé en pouvant gérer les équipes, les joueurs, les matchs, les résultats, les classements et les divisions.

## Prérequis

Assurez-vous d'avoir les éléments suivants installés sur votre machine avant de continuer :

- [PHP](https://www.php.net/downloads.php) >= 7.4
- [Composer](https://getcomposer.org/download/)
- [Symfony CLI](https://symfony.com/download)

## Installation

1. Clonez le dépôt sur votre machine :

```bash
git clone https://github.com/nnaova/sbl-web-app.git
```

2. Allez dans le dossier du projet :

```bash 
cd sbl-web-app
```

3. Installez les dépendances :

```bash
composer install
```

4. Configurez les variables d'environnement :

Dupliquez le fichier `.env` et renommez-le `.env.local`. Modifiez les variables d'environnement selon votre configuration.

5. Créez la base de données :

```bash
php bin/console doctrine:database:create
```

6 effectuez les migrations :

```bash
php bin/console doctrine:migrations:migrate
```

7. Lancez le serveur :

```bash
symfony server:start
```

## Utilisation

Vous pouvez maintenant accéder à l'application à l'adresse suivante : [http://localhost:8000](http://localhost:8000)

## Contributeurs

- [Naova](https://github.com/nnaova)