<!-- omit in toc -->
# Les formulaires

Voyons ensemble comment créer des formulaires HTML pour que vous puissiez récolter les données de vos visiteurs.

Il existe pleins de forme de form (ahah) et toutes sortes d'utilités. Principalement, le but d'un formulaire est de recueillir les informations de votre visiteur et d'ensuite pouvoir les utiliser. Cela peut-être pour l'inscrire et lui donner accès à diverses fonctionnalités sur votre site ou application. Vous pouvez par exemple récupérer son nom et adresse email pour lui envoyer une newsletter ou bien éffectuer un questionnaire concernant la qualité de votre service. Il est également possible de créer un formulaire pour gérer la partie support de votre app et de recevoir les infos directement dans votre compte email.
<!-- omit in toc -->
## Table des matières

- [L'élément \<form>](#lélément-form)
  - [Les attributs du champ \<form>](#les-attributs-du-champ-form)
- [L'élément \<input>](#lélément-input)
  - [Les attributs du champ \<input>](#les-attributs-du-champ-input)
    - [Les attributs communs](#les-attributs-communs)
    - [Attributs spécifique de `text`, `email`,](#attributs-spécifique-de-text-email)
    - [Attributs spécifique de `checkbox` et `radio`](#attributs-spécifique-de-checkbox-et-radio)
    - [Attributs spécifique de `submit`](#attributs-spécifique-de-submit)
    - [Attributs spécifique de `image`](#attributs-spécifique-de-image)
- [L'élément \<button>](#lélément-button)

## L'élément \<form>

Il s'agit d'un élément qui définis un formulaire utilisé pour récupérer les données entrées par votre utilisateur.

```html
<form>
  Les éléments de votre formulaire
</form>
```

### Les attributs du champ \<form>

| Attribut | Description |
|---|---|
|action | L'url du programme qui traitera les informations envoyées par le formulaire.|
|autocomplete | Permet d'autoriser (par défaut) ou non le navigateur à remplir les champs par des informations obtenue précédemment.|
|method | Défini si on utilise la méthode `post`, `get`(par défaut) ou `dialog` pour envoyer les informations au serveur.|
|name | Précise le nom du formulaire, il doit être unique parmi tous les autres formulaires présents sur le même document.|

:closed_book:[En savoir plus](https://developer.mozilla.org/fr/docs/Web/HTML/Element/form)

## L'élément \<input>

C'est l'élement le plus important de votre formulaire. Il permet de définir les champs et leur **type**. Voici une liste avec descriptions de tous les types qui existent.

```html
<input type="text">
<input type="password">
```

| Type | Description |
|---|---|
|**[button](https://developer.mozilla.org/fr/docs/Web/HTML/Element/input/button)**| Un bouton sans comportement propre.|
|**[checkbox](https://developer.mozilla.org/fr/docs/Web/HTML/Element/input/checkbox)**| Une case à cocher qui permet de sélectionner ou désélectionner une valeur.
|**[color](https://developer.mozilla.org/fr/docs/Web/HTML/Element/input/color)**| Permet de définir une couleur.
|**[date](https://developer.mozilla.org/fr/docs/Web/HTML/Element/input/date)**| un contrôle qui permet de saisir une date complète.
|**[email](https://developer.mozilla.org/fr/docs/Web/HTML/Element/input/email)**| Un champ qui permet d'introduire une adresse email.
|**[file](https://developer.mozilla.org/fr/docs/Web/HTML/Element/input/file)**| Permet de sélectionner un fichier. Se complète avec l'attribut `accept` pour préciser quels type de fichiers sont autorisés.
|**[hidden](https://developer.mozilla.org/fr/docs/Web/HTML/Element/input/hidden)**| Permet d'envoyer son contenu sans l'afficher.
|**[image](https://developer.mozilla.org/fr/docs/Web/HTML/Element/input/image)**| Affiche une image comme bouton d'envoie (submit). Il faut préciser les attributs `src` et `alt`. `width` et `height`sont également acceptés.
|**[month](https://developer.mozilla.org/fr/docs/Web/HTML/Element/input/month)**| Permet de saisir un mois et une année.
|**[number](https://developer.mozilla.org/fr/docs/Web/HTML/Element/input/number)**| Permet de saisir un nombre.
|**[password](https://developer.mozilla.org/fr/docs/Web/HTML/Element/input/password)**| Un champ de texte en une seule ligne, qui permet d'introduire un mot de passe dont la valeur est masquée. Les attributs `maxlength`et `minlength`permettent de gérer la taille maximale et minimale.
|**[radio](https://developer.mozilla.org/fr/docs/Web/HTML/Element/input/radio)**| Définis un bouton pour sélectionner un choix parmi plusieurs |
|**[range](https://developer.mozilla.org/fr/docs/Web/HTML/Element/input/range)**| Affiche un contrôleur qui permet de sélectionner un nombre dont la valeur n'est pas importante. |
|**[reset](https://developer.mozilla.org/fr/docs/Web/HTML/Element/input/reset)**| Affiche un bouton qui permet de réinitialiser l'intégralité du formulaire. |
|**[search](https://developer.mozilla.org/fr/docs/Web/HTML/Element/input/search)**| Affiche un champ prévu pour la recherche de termes. Les sauts à la ligne sont retirés automatiquement |
|**[submit](https://developer.mozilla.org/fr/docs/Web/HTML/Element/input/submit)**| Affiche un bouton servant à l'envoi du formulaire |
|**[tel](https://developer.mozilla.org/fr/docs/Web/HTML/Element/input/tel)**| Affiche un champ pour renseigner un numéro de téléphone. |
|**[text](https://developer.mozilla.org/fr/docs/Web/HTML/Element/input/text)**| Définis un champs de texte d'une ligne. Les sauts à la ligne sont retirés automatiquement. |
|**[time](https://developer.mozilla.org/fr/docs/Web/HTML/Element/input/time)**| Permet d'indiquer une valeur de temps. |
|**[url](https://developer.mozilla.org/fr/docs/Web/HTML/Element/input/url)**| Permet d'indiquer une valeur d'url. |
|**[week](https://developer.mozilla.org/fr/docs/Web/HTML/Element/input/week)**| Permet d'indiquer une date représenté par un numéro de semaine et une année. |

:closed_book:[En savoir plus](https://developer.mozilla.org/fr/docs/Web/HTML/Element/input)

### Les attributs du champ \<input>

Nous venons de voir pas mal de type du champ `<input>`, chaque type peux se voir préciser par des attributs. Certains sont communs et d'autres spécifique au type.

```html
<input type="text" value="Saisir votre nom">
<input type="text" value="Saisir votre nom">
```

#### Les attributs communs

| Type | Description |
|---|---|
|[autocomplete](https://developer.mozilla.org/fr/docs/Web/HTML/Element/input#autocomplete) | Indique de le type d'autocomplétion à utiliser.|
|[autofocus](https://developer.mozilla.org/fr/docs/Web/HTML/Element/input#autofocus) | Un booléen qui passe le focus sur le champ lorsqu'on affiche le formulaire.|
|[disabled](https://developer.mozilla.org/fr/docs/Web/HTML/Element/input#disabled) | Un booléen qui indique si le champ est actif ou non.|
|[form](https://developer.mozilla.org/fr/docs/Web/HTML/Element/input#form) | L'identifiant du formulaire auquel se rapporte le champ. Si non précise, se raccroche au formulaire le plus proche.|
|[name](https://developer.mozilla.org/fr/docs/Web/HTML/Element/input#name) | Le nom du champ qui sera rattaché à la valeur envoyée.|
|[readonly](https://developer.mozilla.org/fr/docs/Web/HTML/Element/input#readonly) | Booléen qui permet d'indiquer si le champ est éditable ou non.|
|[required](https://developer.mozilla.org/fr/docs/Web/HTML/Element/input#required) | Booléen qui permet d'indiquer si le champ est nécessaire avant l'envoi ou non.|
|[tabindex](https://developer.mozilla.org/fr/docs/Web/HTML/Element/input#tabindex) | Une valeur numérique qui permet d'indiquer l'ordre dans lequel on passe d'un champ à l'autre avec la touche **tab**.|
|[value](https://developer.mozilla.org/fr/docs/Web/HTML/Element/input#value) | La valeur qui s'affiche dans le champ|

#### Attributs spécifique de `text`, `email`,

| Attribut | Description |
|---|---|
|maxlength | Le nombre maximum de caractères qui peuvent être écrit dans le champ.|
|minlength | Le nombre minimum de caractères qui doivent être écrit pour que le champ soit valide.|
|placeholder | Une valeur qui s'affiche lorsque aucune valeur est rentrée par l'utilisateur.|
|size | Un nombre qui indique combien de caractère doivent s'afficher.|

#### Attributs spécifique de `checkbox` et `radio`

| Attribut | Description |
|---|---|
|checked | Booléen qui indique si le bouton est sélectionné dans le groupe.|

#### Attributs spécifique de `submit`

| Attribut | Description |
|---|---|
|formaction|L'url où envoyez les données du formulaire. Prend la priorité sur l'attribut `action` du formulaire si il est défini.|

#### Attributs spécifique de `image`

| Attribut | Description |
|---|---|
|alt | Comme en HTML, permet d'afficher un texte quand l'image ne s'affiche pas.|
|src | Comme en HTML, permet de définir la source de l'image.|
|height | Défini la hauteur de l'image.|
|width | Défini la largeur de l'image.|

## L'élément \<button>

Pour envoyer votre formulaire on a déjà vu le `type="button"` de l'`input`. Mais ce dernier ne permet pas l'ajout de contenu. Il aura sa `value`mais c'est tout. Sur les navigateurs les plus anciens la balise \<button> peut poser problème (ex: IE6). Mais la majorité des utilisateurs ne devraient pas avoir de soucis.

```html
<button name="button">Click on me :)</button>
```

Peux prendre les attributs suivant: autofocus, disabled, form, formaction, formenctype, formmethod, formnovalidate, formtarget, name, type, value.

* **form**: l'id du formulaire auquel se rattache le bouton. Ainsi il peut être placer en dehors du formulaire.
* **type**: précise si il s'agit d'un bouton `submit`, `reset`, `button`ou `menu`

