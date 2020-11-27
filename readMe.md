# Mise en ligne d'une application avec HEROKU

[Heroku](https://www.heroku.com/)

## Téléchargement et installation
[Documentation](https://devcenter.heroku.com/articles/heroku-cli#download-and-install)

Dans un premier temps, nous allons installer Heroku en local sur notre ordinateur.
De plus, heroku s'appuie sur Git pour son fonctionnement.

Dans votre terminal:
- Mac : `$ brew tap heroku/brew && brew install heroku`.
- Ubuntu : `$ sudo snap install --classic heroku`.
- Windows : Aller sur le lien plus haut.

Si vous avez node.js d'installé, vous pouvez taper ceci dans votre terminal:
`$ npm install -g heroku`

## Aller sur Heroku pour créer un compte

[Suivre ce lien](https://signup.heroku.com/login)


## Création d'une application sur Heroku

Allez dans votre terminal et à la racine de votre projet et tapez: 
- `cd ~/myapp`
- `heroku create`
- `git remote -v` => on vérifie la connexion entre notre repo local et notre nouvel espace sur Heroku.

A la création de notre première app sur Heroku, il va nous demander de nous connecter. Tout est dans la doc plus haut.

## Mettre en ligne

*Héroku n'accepte que les applications. Le point d'entrée de notre site web (index.html) doit avoir un extension correspondant à une techno back-end (php, rb, js, etc...). Nous allons renommer notre fichier de la manière suivante `index.php`.

Pour pusher votre application en ligne, tapez:

- `$ git push heroku master`

- ==> Aller sur votre compte Heroku => setting, pour voir votre site en ligne.

### Heroku et Laravel

Nous hebergerons plus tard nos app Lararel sur Heroku.
- => [An elegant platform for modern PHP apps](https://www.heroku.com/php).