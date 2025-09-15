Instrucciones: 


Requisitos:
Un navegador web moderno (Chrome, Firefox, Edge).
Opcional: Un editor de texto para modificar el código (e.g., VS Code).
Funciona perfecto en dispositivos móviles pero es mejor en versiones de escritorio.

Instalación y Ejecución:
Opción 1:
Clona el repositorio:git clone https://github.com/JulianBuetS/compile-core.git
Abre el archivo Compile-Core.html  en un navegador web.
La aplicación se ejecutará automáticamente, mostrando la interfaz para crear y editar documentos.
Opción 2: 
Abre el bloc de notas o cualquier .txt editor, copia y pega el codigo html de Compile-Core, guardalo con la extensión "html" de manera local. 

Uso Básico:

Crear un documento: Usa el botón "Crear nuevo documento padre" en la interfaz.
Modifica a tu gusto los ejemplos de Lorem Ipsum para que te resulte fluido entender el compilador. Dedicale un tiempo a modificar el orden de los documentos mayores para ver como estos se reordenan automaticamente en los indices mapeados.
Editar metadatos: Ajusta título, compilador y fecha en los campos superiores.
Añadir subdocumentos: Selecciona "Agregar subdocumento" para crear niveles jerárquicos (e.g., doc-1, doc-1a).
Usa el editor de datos para mayor trazabilidad de tu biblioteca.
Exportar: Genera un archivo .txt con estructura jerárquica, metadatos YAML y separadores.
Vista previa: Explora la funcionalidad en https://julianbs.neocities.org/compilecore.

Estructura del Documento:
Los documentos generados incluyen:
Metadatos YAML (título, compilador, fecha).
Jerarquía ramificada (hasta tres niveles topograficos de documentos enlazados con IDs únicos, e.g., doc-1aB).
Formato .txt ligero para parsing eficiente por LLMs y entendible para usuarios.

Contribuir
Haz un fork del repositorio.
Crea una rama para tus cambios:git checkout -b mi-rama
Realiza modificaciones y haz commit:git commit -m "Descripción de los cambios"
Envía un pull request con una descripción clara de las mejoras.
Respeta la licencia MIT del proyecto (ver LICENSE).

Problemas y Soporte
Reporta errores o sugerencias en la sección de Issues de GitHub.
Consulta el README para más detalles sobre la funcionalidad y ventajas.
