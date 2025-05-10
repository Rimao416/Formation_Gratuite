## Qu'est-ce que le HTML ?

HTML signifie **HyperText Markup Language** (Langage de balisage hypertexte). C'est le langage standard utilisé pour créer et structurer le contenu des pages web. Le HTML n'est pas un langage de programmation, mais un langage de balisage qui définit la structure et le contenu d'une page web.

### Rôle du HTML

Le HTML est comme le squelette d'une page web :

- Il organise le contenu (textes, images, vidéos...)
- Il définit la structure sémantique (titres, paragraphes, listes...)
- Il permet de créer des liens entre les pages
- Il intègre d'autres ressources (CSS, JavaScript, médias...)

## Structure de base d'un document HTML

Un document HTML est composé d'éléments, qui sont définis par des balises. Voici la structure de base d'une page HTML :

```html

html
<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Titre de ma page</title>
</head>
<body>
<!-- Le contenu visible de la page va ici -->
    <h1>Mon premier titre</h1>
    <p>Mon premier paragraphe.</p>
</body>
</html>

```

Expliquons chaque partie :

- `<!DOCTYPE html>` : Déclare le type de document (HTML5)
- `<html>` : L'élément racine qui englobe tout le contenu
- `<head>` : Contient les métadonnées (informations sur le document)
    - `<meta charset="UTF-8">` : Définit l'encodage des caractères
    - `<meta name="viewport">` : Optimise l'affichage sur les appareils mobiles
    - `<title>` : Définit le titre de la page (affiché dans l'onglet du navigateur)
- `<body>` : Contient tout le contenu visible de la page
- `<!-- -->` : Commentaires (ignorés par le navigateur)

## Les éléments HTML et leur syntaxe

### Structure d'un élément HTML

La plupart des éléments HTML sont composés de trois parties :

1. **La balise ouvrante** : `<balise>`
2. **Le contenu** : Texte ou autres éléments
3. **La balise fermante** : `</balise>`

Exemple : `<p>Ceci est un paragraphe.</p>`

### Éléments vides

Certains éléments n'ont pas de contenu et donc pas de balise fermante :

- `<img src="image.jpg" alt="Description de l'image">` (pour insérer une image)
- `<br>` (pour un saut de ligne)
- `<hr>` (pour une ligne horizontale)

En HTML5, ces balises peuvent s'écrire sans slash final, bien que `<img />` soit également valide.

### Attributs HTML

Les attributs fournissent des informations supplémentaires sur les éléments :

- Ils sont toujours spécifiés dans la balise ouvrante
- Ils se présentent sous forme de paires nom/valeur : `nom="valeur"`

Exemple : `<a href="https://www.exemple.com" target="_blank">Visiter le site</a>`

Les attributs courants :

- `id` : Identifiant unique pour un élément
- `class` : Classe(s) pour le stylage CSS
- `style` : Styles CSS en ligne
- `src` : Source d'une ressource (image, vidéo...)
- `href` : Référence hypertexte (lien)
- `alt` : Texte alternatif (pour les images)

## Les éléments HTML essentiels

### Titres

HTML propose six niveaux de titres, de `<h1>` (plus important) à `<h6>` (moins important) :

```html

html
<h1>Titre principal</h1>
<h2>Sous-titre</h2>
<h3>Sous-sous-titre</h3>
<!-- etc. jusqu'à h6 -->

```

### Paragraphes et formatage de texte

```html

html
<p>Ceci est un paragraphe de texte.</p>

<p>Ce texte contient <strong>du texte en gras</strong> et <em>du texte en italique</em>.</p>

<p>Voici un <mark>texte surligné</mark> et un <u>texte souligné</u>.</p>

<p>Ceci est du <sub>texte en indice</sub> et du <sup>texte en exposant</sup>.</p>

```

### Listes

**Liste non ordonnée** (à puces) :

```html

html
<ul>
    <li>Élément 1</li>
    <li>Élément 2</li>
    <li>Élément 3</li>
</ul>

```

**Liste ordonnée** (numérotée) :

```html

html
<ol>
    <li>Premier élément</li>
    <li>Deuxième élément</li>
    <li>Troisième élément</li>
</ol>

```

**Liste de définitions** :

```html

html
<dl>
    <dt>HTML</dt>
    <dd>Langage de balisage pour créer des pages web</dd>

    <dt>CSS</dt>
    <dd>Langage de style pour mettre en forme les pages web</dd>
</dl>

```

### Liens

```html

html
<!-- Lien vers une page externe -->
<a href="https://www.exemple.com">Visiter Exemple.com</a>

<!-- Lien vers une page du même site -->
<a href="contact.html">Page de contact</a>

<!-- Lien vers une section de la même page -->
<a href="#section1">Aller à la section 1</a>

<!-- Lien pour télécharger un fichier -->
<a href="document.pdf" download>Télécharger le PDF</a>

<!-- Lien ouvrant dans un nouvel onglet -->
<a href="https://www.exemple.com" target="_blank">Ouvrir dans un nouvel onglet</a>

```

### Images

```html

html
<img src="image.jpg" alt="Description de l'image" width="300" height="200">

```