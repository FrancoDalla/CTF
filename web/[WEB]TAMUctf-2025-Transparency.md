<h1>Enunciado</h1>

I created my own private document sharing site with a novel twist to increase the security boundaries between shared links.

<h2>Resolución</h2>
Al ingresar a la url provista se vio un sitio web para subir y compartir archivos con links privados. La diferencia es que este sitio utilizaria un unico subdominio por cada archivo lo que, según el sitio, provee una capa adicional de seguridad en comparación con los links unicos basados en path.
También en el sitio figuraba un link a un documento de demostración. Tras ver este se probo si estos links a documentos aparecian al buscar por Google. Al no encontrarlo y observar un poco mas el sitio me percate de que este poseía certificados de Let's Encrypt y, por conocimiento previo, sabía que es posible buscar que certificados estan asociados a un dominio mediante distintos buscadores.
Al realizar esto se encontro el link a otro archivo subido al sitio que contenía la flag
gigem{CT_15_41w4y5_w47ch1n9}



<i>Captura del sitio web</i>

![web](https://github.com/user-attachments/assets/545ed2f2-9fef-4a04-9bcf-a845b3594bdd)


<i>Sitio del documento de demostración</i>

![docprueba](https://github.com/user-attachments/assets/b6683284-4f6d-4ea0-beed-5caf8a5595ca)


<i>links asociados a certificados en sitios .transparency.cybr.club</i>

![crt](https://github.com/user-attachments/assets/0181b3d8-dacc-4da5-97c9-16cc144f32ac)


<i>Sitio del documento con la flag</i>

![Captura de pantalla de 2025-04-01 00-46-34](https://github.com/user-attachments/assets/faf40876-1d65-4717-85cc-a535703c4d28)
