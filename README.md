# TP Markdown

Nous allons revoir plusieurs concepts :

-   Le state
-   Les fonctions
-   Le cycles des composants

Nous allons intégrer aussi le localStorage 🎉

Nous allons avoir besoins des packages suivants :

-   [marked](https://www.npmjs.com/package/marked)
-   [bootstrap](https://www.npmjs.com/package/bootstrap)

Ainsi qu'un fichier texte d'exemple qui se trouve [ci contre](sampleText.js)

## Les étapes de création

1. Créer un projet avec create react app
2. Installer les packets npm précédemment cité
    - `npm install marked bootstrap`
3. On charge le CSS de bootstrap
    - Dans index.js on ajoute `import 'bootstrap/dist/css/bootstrap.min.css'`
4. On créer un rendu sur App.js
    - Un coté c'est un `textarea` de l'autre un rendu simple
5. Importer notre donnée `sampleText`
6. Initialiser le state avec `sampleText`
    - Création d'un state qui vaut notre `sampleText`
7. Modification du state via une fonction
    - On créer une fonction `handleChange` qui sera activé à l'événement `onChange` qui vaut le changement de notre state
8. Import de `marked`
9. Utilisation de `marked`
    - `marked(text, { sanitize: true });`
10. Utilisation des cycles de composant pour initialiser le localStorage `componentDidMount` et `componentDidUpdate`
    - `componentDidMount` pour get les informations du localStorage
    - `componentDidUpdate` pour set les informarions dans le localStorage
