# Checklist SEO développeur

Ceci est une checklist à destination du développeur sur les points à vérifier pour faciliter le SEO du projet web. Ne seront donc PAS précisés tous les sujets relevant du designer / rédacteur.

Le référencement moderne implique autant les moteurs de recherche que les réseaux sociaux. Il faut s'assurer que le contenu soit bien interprété par les deux.

## SEO naturel

- [ ] Pas de liste de mots-clés ou de texte cachés dans le contenu via CSS ou JavaScript
- [ ] Pas de liens cassés
- [ ] Pas de contenu obsolète
- [ ] Ajouter `rel="nofollow"` sur les liens réciproques (2 pages de 2 domaines différents se pointant l'une l'autre)
- [ ] Faire supprimer (ou désavouer via Google Search Console) les backlinks de mauvaise qualité
- [ ] Chaque image ou élément non textuel est dotée d'une alternative textuelle (attribut `alt`, 80 caractères max)
- [ ] Chaque contenu audio et vidéo est accompagné de sa transcription textuelle
- [ ] Les textes mis en images sont reproduits dans l'alternative textuelle (attribut `alt`, 80 caractères max)
- [ ] Les termes présents dans l'alternative textuelle des images sont également présents dans le contenu de la page
- [ ] Si le site utilise la technique des jeux de cadres, l'élément NOFRAME est utilisé, décrivant en prose le contenu du cadre. Le mieux reste de ne pas utiliser cette technique du tout
- [ ] Chaque page du site contient un élément de titre de section H1
- [ ] Le contenu visé pour le référencement est mis en exergue (strong ou em)
- [ ] Le contenu de chaque page est organisé selon une structure de titres de section HTML
- [ ] La page d'accueil du site n'est pas une page tunnel
- [ ] La page d'accueil expose la nature des contenus et services proposés
- [ ] L'adresse et le numéro de téléphone de l'entreprise sont disponibles sous forme textuelle
- [ ] Les formats d'images utilisés sont indexables par les principaux moteurs de recherche d'image
- [ ] Le texte des documents PDF internes est sélectionnable
- [ ] Si le site propose un fil de syndication, celui propose des contenus et pas seulement des liens
- [ ] Les images sont cohérentes avec les contenus de la page
- [ ] Le nom de fichier des images significatives est cohérent avec leur contenu
- [ ] Le site propose plusieurs répertoires et/ou sous-domaines
- [ ] Le contenu de chaque nom de domaine lui est propre
- [ ] Chaque langue proposée fait l'objet d'un domaine ou d'un sous-domaine différent (à vérifier)
- [ ] Hors extensions génériques, l'extension du nom de domaine correspond à la zone géographique visée
- [ ] Si le nom de domaine correspond à une zone géographique, le site est hébergé dans cette zone
- [ ] Le libellé de chaque hyperlien décrit sa fonction ou la nature du contenu vers lequel il pointe
- [ ] Les liens qui ne sont pas en rapport avec les contenus ou services proposés sont déclarés en nofollow
- [ ] Les adresses URL ne contiennent pas d'indication concernant les paramètres de session
- [ ] Les URL des liens internes contiennent exclusivement des caractères alphanumériques ou considérés comme sûrs
- [ ] Les liens externes sont en rapport avec les contenus ou services proposés
- [ ] Les URL contiennent des termes présents dans les titres de pages
- [ ] Le nombre de liens externes dans une page n'excède pas le nombre de liens internes
- [ ] Des libellés de liens identiques pointent vers la même page
- [ ] Tous les hyperliens du site sont valides
- [ ] Les liens internes utilisent une URL unique pour chaque page
- [ ] Le titre de chaque page (élément TITLE) permet d'identifier son contenu (80 caractères max)
- [ ] Le contenu de l'élément TITLE de chaque page ne commence pas par le nom du site
- [ ] Le contenu de l'élément meta description est une phrase significative et non une liste de mots clefs (250 caractères max)
- [ ] Le code source de chaque page indique la langue principale du contenu
- [ ] Le site compte autant de meta description différentes que de pages
- [ ] Le site propose un plan du site contenant des liens HTML
- [ ] L'accès aux contenus significatifs n'est pas conditionné par des actions de formulaires
- [ ] L'accès aux contenus significatifs n'est pas conditionnée par le support de javascript
- [ ] L'accès aux contenus significatifs n'est pas conditionné par le support des cookies
- [ ] La racine du site contient des instructions pour les robots d'indexation (fichier robots.txt)
- [ ] Le fichier robots.txt propose une référence valide à un fichier sitemap
- [ ] Le site propose un fichier sitemap indiquant les contenus à explorer
- [ ] Le temps de rafraichissement indiqué dans le fichier sitemap est cohérent avec la fréquence de mise à jour du site
- [ ] Le site fait l'objet de liens entrants
- [ ] Le site n'interdit pas la mise en place de liens entrants
- [ ] Le plan du site est accessible depuis la page d'accueil
- [ ] Les libellés du menu principal de navigation sont cohérents avec le contenu des rubriques
- [ ] Les menus sont utilisables sans extension (flash...) ou activation de langages (CSS ou JavaScript..)
- [ ] Le site propose un fil d'Ariane
- [ ] Le site ne contient pas de liens vers des pages en construction
- [ ] Les vidéos sont soumises à au moins deux diffuseurs externes
- [ ] Les contenus du site sont consultables sans extension (flash...) ou activation de langages (CSS ou JavaScript..)
- [ ] Les styles ne sont pas utilisés pour générer du contenu
- [ ] Les mises en majuscules à des fins décoratives sont effectuées à l'aide des styles CSS
- [ ] Les textes pouvant être mis en forme via des styles ne sont pas remplacés par des images
- [ ] Les contenus HTML sont mis en forme à l'aide de styles CSS externalisés
- [ ] Si le site propose des redirections, celles-ci sont permanentes (code 301)
- [ ] Le serveur envoie un code HTTP 404 pour les ressources non trouvées
- [ ] Les URL alternatives vers la page d'accueil font l'objet d'une redirection 301 vers l'URL principale
- [ ] Les noms de domaine secondaires redirigent en 301 vers le nom de domaine principal
- [ ] Le site et le serveur sont configurés pour délivrer les pages de manière performante

## Méta Données

### Quelques outils pour bien travailler

- [Google Structured Data Testing Tool](https://search.google.com/structured-data/testing-tool/u/0/)
- [SEO META chrome extension](http://www.seo-extension.com/)
- [Facebook OpenGraph debugger](https://developers.facebook.com/tools/debug/)
- [Twitter Card Validator](https://cards-dev.twitter.com/validator)
- [Pinterest Rich Card debugger](https://developers.pinterest.com/tools/url-debugger/)

### OpenGraph

Voici une bonne base documentée à copier-coller dans votre code en remplaçant les valeurs. Pour aller plus loin, voir la doc de [The Open Graph protocol](https://ogp.me/).

```html
<!-- OpenGraph, à placer sous la balise <title> -->
<!-- Pour plus d'informations : https://ogp.me/ -->
<!-- Titre : penser à faire un titre assez court qui décrit bien la page, comme pour le SEO classique -->
<meta property="og:title" content="SEO pour les Samouraïs" />

<!-- Description : Une description 100% texte (donc pas de liens), très similaire à la meta description classique -->
<meta
  property="og:description"
  content="Une description 100% texte (donc pas de liens), très similaire à la meta description classique"
/>

<meta property="og:type" content="article" />

<!-- URL : URL cannonique, version desktop, sans variable de session, sans pagination ou autre compteur, cette URL ne devrait jamais changer (en utilisant généralement un uid) -->
<meta property="og:url" content="http://www.example.com/article/tt0117500/" />

<!-- Image : attention, si vous souhaitez changer cette image avec le temps, bien penser à changer l'URL de l'image aussi (avec un paramètre de requête ?v=27365 par exemple), car Facebook les téléchargent une fois pour toutes. taille recommandée : 1200 par 630 -->
<meta property="og:image" content="http://example.com/images/seo.jpg" />
<meta property="og:image:type" content="image/jpeg" />
<meta property="og:image:width" content="1200" />
<meta property="og:image:height" content="630" />

<!-- Partie spécifique à Twitter -->
<!-- Pour plus d'infos : https://developer.twitter.com/en/docs/tweets/optimize-with-cards/guides/getting-started -->
<!-- Format du média riche affiché, voir la doc pour les possibilités -->
<meta name="twitter:card" content="summary_large_image" />

<!-- Compte twitter du site cannonique (a qui appartient le domaine) -->
<meta name="twitter:site" content="@site" />

<!-- Compte twitter du créateur du contenu de la page précise -->
<meta name="twitter:creator" content="@creator" />

<!-- Image spécifique pour twitter, 150 par 150 pour le type summary, 560 par 300 pour summary_large_image -->
<meta name="twitter:image" content="http://example.com/images/seo.jpg" />
```

## Données structurées

Voici un exemple qui remplace l'URL dans les résultats de recherche par un fil d'ariane. À placer dans le `<body>`. Le code est copié depuis la [documentation de Google sur les Données structurées](https://developers.google.com/search/docs/data-types/breadcrumb).

Créez une nouvelle balise `<script>` pour chaque bloc de données structurées.

```html
<script type="application/ld+json">
  {
    "@context": "https://schema.org",
    "@type": "BreadcrumbList",
    "itemListElement": [
      {
        "@type": "ListItem",
        "position": 1,
        "name": "Books",
        "item": "https://example.com/books"
      },
      {
        "@type": "ListItem",
        "position": 2,
        "name": "Authors",
        "item": "https://example.com/books/authors"
      },
      {
        "@type": "ListItem",
        "position": 3,
        "name": "Ann Leckie",
        "item": "https://example.com/books/authors/annleckie"
      }
    ]
  }
</script>
```

## Optimisations mobiles

Google dispose désormais de 2 index différents : un pour les résultats mobiles, et un autre pour le reste (principalement les résultats desktop).

Il est donc primordial de faire attention à soigner et optimiser l'aspect mobile de votre projet web.

- [ ] Une méta viewport bien calibrée : `<meta name="viewport" content="width=device-width, user-scalable=no, initial-scale=1">`
- [ ] Si vous créez une PWA, alors vous pouvez ajouter [les meta tags spécifiques Apple](https://developer.apple.com/library/archive/documentation/AppleApplications/Reference/SafariHTMLRef/Articles/MetaTags.html) ainsi qu'un [manifest.json](https://developers.google.com/web/fundamentals/web-app-manifest/)
- [ ] Générez toutes les icones pour les différents appareils mobiles sur [Real Favicon Generator](https://realfavicongenerator.net/)
- [ ] Lancez un audit sur [Lighthouse](https://developers.google.com/web/tools/lighthouse/) et atteignez un score le plus élevé possible (80 est un minimum)

## Outils SEO généralistes

Ces outils ne sont pas là pour aider le développeur mais le marketer. Je les ajoute tout de même car cela fait un très bon complément à cette checklist.

- [WooRank](https://www.woorank.com/fr) : outil complet et généraliste, interface très agréable, priorisation des actions à mener, génération de rapports pdf
- [Google Keyword Planner](https://ads.google.com/intl/fr_fr/home/tools/keyword-planner/) : Pour affiner son choix de mots-clés afin de sortir des termes trop génériques
- [Google Trends](https://trends.google.fr/trends/?geo=FR) : afin de comparer l'évolution de popularité des mots-clés
- [Google Search Console](https://search.google.com/search-console/about) : pour surveiller l'état des recherches et des liens, permets de vérifier s'il y a des backlinks depuis des mauvais sites (spam)
- [SpyFu](https://www.spyfu.com/) : découvrez la stratégie de mots clés de vos concurrents

## Inspirations :

- [Opquast checklist](https://checklists.opquast.com/seo/)
- [ibandominguez SEO checklist](https://github.com/ibandominguez/seo-checklist)
- [TutsPlus SEO checklist](https://github.com/tutsplus/SEO-Checklist-for-Web-Designers/blob/master/seo_checklist.md)
- [FrontEnd Masters Modern SEO course](https://frontendmasters.com/courses/modern-seo/introduction/)
- [HTML5 Boilerplate](https://github.com/h5bp/html5-boilerplate)
