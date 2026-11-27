# Design UI UX — AI Agent Skill for HTML + Tailwind Prototypes

[English](README.md) | [简体中文](README.zh-CN.md) | [繁體中文](README.zh-TW.md) | [日本語](README.ja.md) | [한국어](README.ko.md) | [Español](README.es.md) | Français | [Deutsch](README.de.md)

Créez des prototypes UI/UX avec HTML + Tailwind. Recherchez des références visuelles, choisissez un style et générez des pages à prévisualiser dans votre navigateur.

## Installation

Installez avec npx, de préférence dans votre projet :

```bash
npx skills add ducafecat/design-ui-ux
```

## Utilisation

### 1. Rechercher des références visuelles

Préparez un document de spécifications produit (PRD) précisant le produit, son public et les écrans nécessaires. Saisissez ensuite :

```text
/design-ui-ux Crée une interface mobile dans le style de Xiaohongshu.

Référence :
docs/prd.md
```

![Recherche de références visuelles](images/1795618228981.png)

### 2. Choisir une direction visuelle

Choisissez une proposition. Si aucune ne convient, demandez une nouvelle sélection :

```text
Montre-moi une autre sélection de références.
```

![Choix de la direction visuelle](images/1795618428611.png)

### 3. Créer le prototype

Saisissez le numéro de la référence choisie, par exemple B2. Choisissez ensuite un style parmi les options proposées, par exemple la première.

![Sélectionnez une référence et examinez les styles proposés.](images/1795618786169.png)

```text
B2
```

![Sélectionnez une référence et examinez les styles proposés.](images/1795619134358.png)

Exemple pour choisir la première option :

```text
1
```

Après confirmation, le prototype est enregistré dans `design/index.html`. Ouvrez-le dans votre navigateur pour le prévisualiser.

![Prototype terminé](images/1795620741606.png)

### 4. Afficher les écrans côte à côte

Pour examiner tous les écrans ensemble, saisissez :

```text
Dispose les vues de design/index.html côte à côte et enregistre-les dans design/平铺.html.
```

Fichier créé : `design/平铺.html`

![Écrans côte à côte](images/1795620965224.png)

### 5. Comparer plusieurs propositions

Si vous hésitez entre plusieurs styles, créez une page d’accueil pour chacun et comparez-les :

```text
Crée une page d’accueil pour chacune des options 1, 2, 3 et 4, puis enregistre-les dans design/compare.html.
```

Fichier créé : `design/compare.html`

![Quatre propositions de design](images/1795619938511.png)

## Prérequis

- L’installation nécessite Node.js 22.20 ou ultérieur ainsi que npm / npx. Les pages HTML générées ne nécessitent pas Node.js.
- La recherche locale nécessite Python 3, sans paquet tiers. Sans Python, vous pouvez suivre les consignes de design pour créer des pages, mais la recherche locale est indisponible.
- La recherche de références et la vérification des pages nécessitent un navigateur prenant en charge les captures d’écran et la prévisualisation de fichiers HTML locaux. Ego Lite est utilisé par défaut et nécessite de configurer séparément la compétence `ego-browser`. Un autre navigateur peut être utilisé selon les instructions de la compétence.
- Tailwind doit être compilé pendant le développement. Compilez-le avant livraison afin que le HTML final s’ouvre sans Node.js, CDN ni compilation à l’exécution.

## Retours, maintenance et licence

Lisez [CONTRIBUTING.md](CONTRIBUTING.md) avant de proposer des améliorations. Consultez [CHANGELOG.md](CHANGELOG.md) pour l’historique et [SECURITY.md](SECURITY.md) pour les problèmes sensibles. Signalez les problèmes reproductibles dans [GitHub Issues](https://github.com/ducafecat/design-ui-ux/issues).

Le projet ne dispose pas encore de licence définie. Vérifiez les autorisations applicables avant de l’utiliser ou de le redistribuer. Avant publication, le responsable doit vérifier les sources, les droits de redistribution et les licences du code et des données. La mention d’une source ne vaut pas autorisation de redistribution. Consultez la [notice sur les sources](NOTICE.md).
