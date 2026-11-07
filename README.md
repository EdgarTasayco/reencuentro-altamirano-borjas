# Familia Altamirano Borjas · Archivo de recuerdos

Web estática, responsive y lista para GitHub Pages. No requiere servidor ni base de datos.

## Probar localmente
Abre `index.html` con Chrome o Edge. No necesitas instalar nada.

## Conectar Google Drive
1. Sube cada MP4 a Drive y espera a que termine el procesamiento.
2. En cada archivo: **Compartir > Acceso general > Cualquier persona con el enlace > Lector**.
3. Copia el enlace del archivo (por ejemplo, `https://drive.google.com/file/d/ABC123/view?usp=sharing`).
4. Edita `assets/js/recuerdos.js` y pega cada enlace en `driveUrl` del capítulo correspondiente.
5. Guarda y prueba los botones de reproducción.

## Publicar en GitHub Pages
1. Crea un repositorio **público** en GitHub llamado `reencuentro-altamirano`.
2. Sube `index.html` y la carpeta `assets` a la **raíz** del repositorio (no subas el ZIP sin extraer).
3. En **Settings > Pages > Build and deployment**, selecciona **Deploy from a branch**, rama `main`, carpeta `/(root)` y guarda.
4. Espera a que GitHub muestre la URL, normalmente `https://TU_USUARIO.github.io/reencuentro-altamirano/`.

## Agregar un nuevo año
Edita solo `assets/js/recuerdos.js`: agrega un objeto al arreglo `window.RECUERDOS` con `year`, `title`, `description` y `chapters`. Cada capítulo tiene `title`, `subtitle`, `description`, `cover` y `driveUrl`. El selector de años se genera automáticamente.

## Privacidad y límites
El sitio es público y los videos de Drive configurados como «cualquier persona con el enlace» son accesibles por quien obtenga el enlace. GitHub Pages no ofrece control de acceso privado. Google Drive puede tardar en procesar archivos grandes o limitar su reproducción; comprueba en varios dispositivos. El diseño usa paisajes ilustrados con CSS, sin fotos externas ni fuentes remotas.
