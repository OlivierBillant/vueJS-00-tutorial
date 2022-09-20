# VueJS

## Introduction
----
Lightweight
Progressive : usable anywhere, can replace JQuery.  
Incrementally adoptable : can update one page after another.
Started in 2014. Since : Top 3 JS framework.    
Vue3 : 2020.

## Utilisation via cdn
Dans une structure html basique :
- Ajout du CDN
``` html
 <script src="https://unpkg.com/vue@3/dist/vue.global.js"></script>
```
- Création d'une "app" vue dans une balise script dédiée
- Création d'une div dans laquelle sera représentée l'app
- Association de l'app avec la div par son id

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <title>Vue 3 basics</title>
  </head>
  <body>
    <div id="app">
      <!-- Hello Vue3 -->
      <!-- On appelle dans un second temps directement la variable déclarée dans data. -->
      {{greeting}}
    </div>

    <!-- On appelle VueJS en cdn -->
    <script src="https://unpkg.com/vue@3/dist/vue.global.js"></script>
    <script>
      // Creation d'une vue
      let app = Vue.createApp({
        data: function () {
          return {
            greeting: "Hello Vue 3 !!!",
          };
        },
      });

      // Lie la vue avec la div protant l'id app.
      app.mount("#app");
    </script>
  </body>
</html>
```
