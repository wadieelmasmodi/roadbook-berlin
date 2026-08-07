# Roadbook Paris → Berlin → Paris

Carnet de route interactif pour un aller-retour en voiture Paris–Berlin, du 9 au 18 août 2026.

**Page publiée :** https://wadieelmasmodi.github.io/roadbook-berlin/

## Contenu

Une page (`index.html`), un dossier `img/` de photos d'hôtels et deux frises SVG, sans dépendance ni build :

- programme heure par heure sur 10 jours, une journée affichée à la fois
- carte par journée avec fond de plan, étapes numérotées et échelle
- photo et lien Google Maps sur chaque lieu
- parkings hors zone environnementale allemande (véhicule sans plaque verte)
- thème clair / sombre suivant celui du navigateur

## Ressources externes

Le texte, les liens et la structure fonctionnent hors ligne. Deux choses nécessitent une connexion :

- les fonds de carte, servis par [CARTO](https://carto.com/) à partir des données [OpenStreetMap](https://www.openstreetmap.org/copyright)
- les photos des lieux, servies par Wikimedia Commons

Les photos d'hôtels font exception : elles sont stockées dans `img/` et proviennent des
établissements eux-mêmes, donc elles s'affichent hors ligne. Chaque image porte sa source
en légende. Pour en remplacer une, écrasez le fichier dans `img/` en gardant le même nom.

La silhouette des neuf étapes du bandeau est aussi exportée en fichiers autonomes et
réutilisables, sans les noms de villes (`frise.svg`, `frise.png`) et avec (`frise-villes.svg`,
`frise-villes.png`). La page ne s'en sert pas — elle garde sa copie inline — donc les modifier
ne casse rien.

Tous portent le fond `#22252A` du bandeau, sans lequel les silhouettes gris clair seraient
invisibles sur blanc. Dans les SVG, supprimez le `<rect>` en tête de fichier pour un fond
transparent. Les PNG sont rendus en 2400 px de large, soit le double de la taille de dessin.

## Modifier

Éditez `index.html` et poussez sur `main` : GitHub Pages redéploie tout seul.
