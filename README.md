# Documentacion_Terming_en_linea
Documentación actualizable de la Empresa Terming SPA

📄 TermIng — Repositorio Documental HSE en Línea
Este repositorio contiene la página web documental del Sistema de Gestión HSE de TermIng Chile SPA. Su objetivo es proporcionar a los trabajadores, contratistas y colaboradores un acceso rápido, organizado y transparente a toda la documentación oficial de Seguridad, Salud Ocupacional y Gestión HSE.

🌐 Sitio en vivo
🔗 https://TermingChile.github.io/Documentacion_Terming_en_linea

📂 Estructura del repositorio
Archivo	Función
index.html	Página web principal (estructura, estilos, lógica de presentación).
documentos.json	Base de datos de todos los documentos del sistema (código, nombre, estado, URL del PDF).
README.md	Este archivo, con instrucciones para el mantenimiento.
🚀 Cómo actualizar la documentación
Cuando agregues un nuevo PDF al sistema (o actualices el estado de uno existente), sigue estos pasos:

Sube el PDF a la carpeta correspondiente en Google Drive.

Obtén el enlace público del archivo:

Haz clic derecho → "Compartir" → "Cualquier persona con el enlace" → Copiar URL.

Edita el archivo documentos.json en este repositorio (puedes hacerlo directamente desde la web de GitHub).

Busca el documento por su código (ej. "PO-PR-005").

Actualiza los campos:

"status": "pending" → "status": "ready"

"url": null → "url": "https://drive.google.com/file/d/..."

Guarda los cambios (Commit) con un mensaje claro, por ejemplo: "Añadido PDF de PO-PR-005".

Espera ~30 segundos y recarga la página web. Los cambios aparecerán automáticamente.

⚠️ Nota: Los documentos con "status": "pending" y "url": null se muestran como "⏳ Pendiente" y no tienen enlace activo. Cuando estén listos, solo hay que cambiar esos dos valores.

📋 Estructura del archivo documentos.json
El archivo sigue este formato:

json
{
  "documentos": [
    {
      "category": "1. GOBERNANZA Y POLÍTICAS",
      "items": [
        {
          "code": "SG-PR-001",
          "name": "Política de Seguridad y Salud Ocupacional",
          "status": "ready",
          "url": "https://drive.google.com/file/d/XXXX/view"
        }
      ]
    }
  ]
}
category: nombre de la categoría (según el LOG Maestro).

code: código único del documento.

name: nombre descriptivo.

status: "ready" (disponible) o "pending" (en desarrollo).

url: enlace público al PDF en Google Drive (o null si no existe).

🛠️ Tecnologías utilizadas
HTML5 + CSS3 – Estructura y diseño responsive.

JavaScript (ES6) – Carga dinámica de datos, buscador y filtros.

JSON – Almacenamiento de los datos documentales.

GitHub Pages – Hosting gratuito y actualización automática.

📎 Enlaces de interés
Google Drive HSE – Carpeta principal

LOG Maestro de Documentos – (incluido en el repositorio como referencia)

👥 Mantenimiento
Este repositorio es mantenido por el equipo de TermIng Chile SPA. Cualquier duda o sugerencia, contactar a:

📧 Termingchile@protonmail.com

📲 +569 64844180

📜 Licencia
Este proyecto es de uso interno de TermIng Chile SPA y no está sujeto a licencia pública. Su reproducción no autorizada está prohibida según la Ley 19.628 de Protección de la Vida Privada.

TermIng Chile SPA – Seguridad, precisión y confianza en cada documento.
