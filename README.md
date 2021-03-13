# Para compilar el SCSS automaticamente:

## 1. Descargar esta extension https://marketplace.visualstudio.com/items?itemName=ritwickdey.live-sass.

## 2. Añade esta configuración en el settings.json de vs code:

```

  "liveSassCompile.settings.formats": [

    {
      "format": "compressed",
      "extensionName": ".min.css",
      "savePath": "/styles/css"
    }

  ]

```

## 3. Ve al archivo main.scss en `/styles/scss` y haz click en el boton de la barra inferior de vs code "Watch Sass":

### 3.1 Esto creara una carpeta css dentro de `/styles` con un archivo css minificado.

## 4 Usa este comando para ignorar el `main.css.min.map`

```

git update-index --assume-unchanged styles/css/main.min.css.map

```

## 4. Listo ya puedes abrir el proyecto con live server, no hay que hacer mas nada que seguir creando codigo sass porque se compilara todo automaticamente desde main.scss.
