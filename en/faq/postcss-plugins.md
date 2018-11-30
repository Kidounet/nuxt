---
title: Plugins PostCSS
description: Comment utiliser des plugins PostCSS ?
---

# Comment utiliser des plugins PostCSS ?

Dans votre fichier `nuxt.config.js` :

```js
export default {
  build: {
    postcss: {
      // Ajoutez le nom du plugin en cl� et les arguments en valeur
      // Installez-les avant comme d�pendance avec npm ou yarn
      plugins: {
        // d�sactivez un plugin en passant false comme valeur
        'postcss-url': false,
        'postcss-nested': {},
        'postcss-responsive-type': {},
        'postcss-hexrgba': {}
      },
      preset: {
        // Changer le param�trage de postcss-preset-env
        autoprefixer: {
          grid: true
        }
      }
    }
  }
}
```
