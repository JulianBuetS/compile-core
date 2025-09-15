# compile-core
Compilador de documentos para trabajo usuarios/LLM
Compile-Core es un compilador web auto-portable que genera repositorios unificados de documentos navegables optimizados para LLMs. Su estructura jerárquica (documentos ramificados) con metadatos YAML y separadores asegura compatibilidad y navegabilidad simplificada para generar documentos extensos plenamente navegables por IA sin que estas pierdan especificidad o divaguen demasiado en encontrar lo que se les solicita o aquello que deberian recordar de manera persistente durante una o varias sesiones de trabajo. La modularidad de contenidos editables permite reorganizar índices automáticamente (e.g., doc-1, doc-1a), ahorrando tiempo significativo frente a editores de texto simple tradicionales, donde la reindexación manual es laboriosa y desgastante. Los formatos de salida .txt son ligeros, económicos y diseñados para parsing eficiente por LLMs, preservando contexto mediante IDs únicos.
¿Por qué es mejor que un editor de texto simple?
A diferencia de editores estándares, Compile-Core estructura documentos con jerarquía, enlaces internos y módulos editables, facilitando la navegación y el procesamiento, esto es ideal para cuando se necesita trabajar con una IA basada en LLM sobre documentos extensos o cuando hay que estructurar para el abordaje del mismo un entorno minimo de rigurosidad. Compile-Core es una aplicación web autoportable que organiza datos con metadatos editables (título, compilador, fecha) y índices automáticos, reduciendo ambigüedad y acortando en gran escala esfuerzo manual. La modularidad permite ajustes dinámicos sin reeditar índices, ni poniendo en riesgo la navegación, optimizando flujos de trabajo complejos. Su interfaz es intuitiva y sensilla superando las limitaciones de editores lineales para documentación en formato .txt que sorprendentemente iguala y a veces supera la utilidad de editores Markdown estáticos gracias a su capacidad de edición en tiempo real.

(Ejemplo usando el clasico Lorem Ipsum para mayor ilustratividad)

---
title: Compilación de Documentos
description: Biblioteca jerárquica navegable
compiler: Julián Buet Scarcella
date: 2025-09-15
authors:
  - Julián Buet Scarcella, Leliel (AI) 
version: 1.0.0
documents:
  - id: doc-1
    title: ¿Qué es Lorem Ipsum?
  - id: doc-2
    title: Definición
    subdocuments:
      - id: doc-2a
        title: ¿Por qué lo usamos?
        sub-subdocuments:
          - id: doc-2aB
            title: Aplicaciones Prácticas
  - id: doc-3
    title: Traducción de H. Rackham
---

=Índice=
==1. ¿Qué es Lorem Ipsum?== (#doc-1)
==2. Definición== (#doc-2)
===2a. ¿Por qué lo usamos?=== (#doc-2a)
====2aB. Aplicaciones Prácticas==== (#doc-2aB)
==3. Traducción de H. Rackham== (#doc-3)
-------------------------------

==1. ¿Qué es Lorem Ipsum?== [#doc-1]
Al contrario del pensamiento popular, el texto de Lorem Ipsum no es simplemente texto aleatorio. Tiene sus raíces en una pieza clásica de la literatura del Latín, que data del año 45 antes de Cristo, haciendo que este adquiera más de 2000 años de antigüedad.
Lorem Ipsum es simplemente el texto de relleno de las imprentas y archivos de texto. Lorem Ipsum ha sido el texto de relleno estándar de las industrias desde el año 1500, cuando un impresor desconocido usó una galería de textos y los mezcló de tal manera que logró hacer un libro de textos especimen. No sólo sobrevivió 500 años, sino que también ingresó como texto de relleno en documentos electrónicos, quedando esencialmente igual al original. Fue popularizado en los 60s con la creación de las hojas "Letraset", las cuales contenían pasajes de Lorem Ipsum, y más recientemente con software de autoedición, como por ejemplo Aldus PageMaker, el cual incluye versiones de Lorem Ipsum.
-------------------------------

==2. Definición== [#doc-2]
Lorem Ipsum: "Neque porro quisquam est qui dolorem ipsum porque dolor sit amet, consectetur, adipisci velit..." - Nadie ama al dolor, simplemente por que es dolor".
===2a. ¿Por qué lo usamos?=== [#doc-2a]
Es un hecho establecido hace demasiado tiempo que un lector se distraerá con el contenido del texto de un sitio mientras que mira su diseño. El punto de usar Lorem Ipsum es que tiene una distribución más o menos normal de las letras, al contrario de usar textos como por ejemplo "Contenido aquí, contenido aquí".
====2aB. Aplicaciones Prácticas==== [#doc-2aB]
Este elemento textual sirve para infinidad de cuestiones relativas a pruebas de texto y funcionalidad.
-------------------------------

==3. Traducción de H. Rackham== [#doc-3]
But I must explain to you how all this mistaken idea of denouncing pleasure and praising pain was born and I will give you a complete account of the system, and expound the actual teachings of the great explorer of the truth, the master-builder of human happiness. No one rejects, dislikes, or avoids pleasure itself, because it is pleasure, but because those who do not know how to pursue pleasure rationally encounter consequences that are extremely painful. Nor again is there anyone who loves or pursues or desires to obtain pain of itself, because it is pain, but because occasionally circumstances occur in which toil and pain can procure him some great pleasure. To take a trivial example, which of us ever undertakes laborious physical exercise, except to obtain some advantage from it? But who has any right to find fault with a man who chooses to enjoy a pleasure that has no annoying consequences, or one who avoids a pain that produces no resultant pleasure?
-------------------------------
