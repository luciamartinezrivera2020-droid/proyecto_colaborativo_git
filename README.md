Prueba Colaborativa Git B

Reflexión sobre el conflicto en README.md

El conflicto fue causado porque dos personas editaron la misma línea del README al mismo tiempo y luego intentaron subir sus cambios al repositorio remoto. Git no podía decidir automáticamente cuál versión mantener, por eso apareció el conflicto.
Para resolverlo, seguimos estos pasos:
Intentamos hacer git push y recibimos un error indicando que había cambios en el remoto que no teníamos.
Ejecutamos git pull origin main para traer los cambios del remoto.
Git mostró los marcadores de conflicto (<<<<<<<, =======, >>>>>>>) en el archivo.
Editamos manualmente el README, eligiendo qué contenido conservar o combinando ambos cambios.
Guardamos el archivo, hicimos git add README.md y git commit -m "Resuelve conflicto de sincronización".
Finalmente, subimos los cambios con git push origin main y verificamos que todo estaba sincronizado.
Este proceso nos enseñó que los conflictos ocurren cuando varias personas trabajan en las mismas líneas y que Git nos permite resolverlos de forma manual para mantener el historial de trabajo de todos.

