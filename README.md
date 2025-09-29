# Leyes Auditoras CDMX - Base de Conocimiento para IA

Este repositorio es una base de conocimiento curada, diseñada específicamente para el entrenamiento y la operación de Modelos de Lenguaje Grandes (LLMs) y agentes de IA enfocados en la auditoría y el marco legal de la Ciudad de México.

El objetivo es proporcionar datos estructurados y accesibles que permitan a los sistemas de IA navegar, comprender y analizar la compleja red de leyes y normativas que rigen la fiscalización y la administración pública en la CDMX.

## Estructura del Repositorio

El proyecto está organizado en dos directorios principales:

1.  `fuentes_oficiales/`: Contiene los documentos originales en formato PDF tal como fueron publicados en las gacetas oficiales. Sirve como fuente de verdad y para verificación.

2.  `marco_legal_auditoria_cdmx/`: Es el núcleo de la base de conocimiento, donde las leyes están procesadas y estructuradas para el consumo de la IA. La jerarquía sigue un orden lógico y legal:

    *   **`1_constitucional/`**: La Constitución Política de la Ciudad de México, que es la norma fundamental.
    *   **`2_ley_principal_fiscalizacion/`**: La Ley de Fiscalización Superior, que es el eje central de la auditoría gubernamental.
    *   **`3_leyes_complementarias/`**: Un conjunto de leyes que abordan áreas específicas y complementan la ley principal. Incluye:
        *   `adquisiciones/`
        *   `austeridad_y_ejercicio_recursos/`
        *   `control_interno/`
        *   `responsabilidades/`
    *   **`4_normatividad_administrativa/`**: Regulaciones y circulares que detallan la aplicación de las leyes en la operación diaria.

### Formato de los Datos

Dentro de cada subdirectorio en `marco_legal_auditoria_cdmx/`, encontrarás dos tipos de archivos:

*   **`.txt`**: Un archivo de texto plano que contiene el texto íntegro de la ley. Este formato es ideal para el procesamiento de lenguaje natural (NLP) y para que los modelos de IA lo analicen.
*   **`meta.json`**: Un archivo JSON con metadatos clave sobre la ley, como su nombre completo, fecha de publicación, última reforma, etc. Esto permite a los agentes obtener información contextual rápidamente sin necesidad de procesar todo el texto.

## Uso con Agentes de IA y MCP (Model Context Protocol)

La estructura de este repositorio está optimizada para ser utilizada por agentes de IA que implementan el Protocolo de Contexto de Modelo (MCP). Un agente puede:

1.  **Explorar la estructura de directorios** para entender el panorama legal.
2.  **Leer los archivos `meta.json`** para obtener contexto y datos clave de forma eficiente.
3.  **Realizar búsquedas semánticas** en los archivos `.txt` para encontrar artículos o disposiciones específicas.
4.  **Validar y cruzar información** entre diferentes normativas para realizar análisis complejos.

## Contribuciones

Las contribuciones son bienvenidas. Si deseas agregar nuevas leyes, actualizar las existentes o mejorar los metadatos, por favor, sigue la estructura de directorios y formatos existentes.

