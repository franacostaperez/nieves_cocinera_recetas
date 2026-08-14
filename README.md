# Catálogo remoto de Nieves cocinera

Esta carpeta está lista para publicarse en GitHub Pages. `recipes.json` es el archivo que consulta la aplicación automáticamente al arrancar.

## Publicarlo

1. Crea en GitHub un repositorio público, por ejemplo `nieves-cocinera-recetas`.
2. Sube `recipes.json` a la raíz del repositorio.
3. En **Settings > Pages**, elige **Deploy from a branch**, rama **main** y carpeta **/(root)**.
4. Espera a que GitHub muestre la dirección publicada. Será parecida a:
   `https://TU_USUARIO.github.io/nieves-cocinera-recetas/recipes.json`
5. En la aplicación abre **Más > Ajustes**, pega esa dirección en **Dirección recipes.json** y cierra la aplicación por completo.
6. Al volver a abrirla, se actualizará sola. No hay botón de actualización.

## Añadir o modificar recetas

- Usa `recipes.example.json` como plantilla para cada receta nueva.
- Añade las recetas dentro de la lista `recipes` de `recipes.json`.
- Cada receta debe conservar siempre el mismo `id`.
- Aumenta `revision` cuando cambies una receta ya publicada.
- Aumenta `catalogVersion` cada vez que publiques una tanda de cambios.
- Una fotografía puede guardarse en el repositorio e indicarse con su dirección HTTPS en `imageURL`.
- Valida el JSON antes de publicarlo: una coma o comilla incorrecta impide leer todo el catálogo.

Si no hay conexión, la aplicación conserva las recetas que ya tenía guardadas y vuelve a intentarlo en el siguiente arranque.
