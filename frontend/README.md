---

# backend/README.md

# Backend de SOCION

El módulo **Backend** de SOCION constituye el núcleo lógico del proyecto, encargado de procesar datos, ejecutar simulaciones y servir resultados al frontend de manera eficiente y segura.

## Objetivo

Garantizar la correcta gestión de la lógica de negocio, la exposición de endpoints y la integración con la IA para la generación de análisis narrativos de manera escalable y mantenible.

## Estructura Detallada

* `main.py` → Punto de entrada de la API.
* `models/` → Definición de estructuras y clases de datos.
* `routes/` → Endpoints REST para la interacción con el frontend.
* `services/` → Lógica de simulación y generación de análisis narrativo.
* `utils/` → Funciones auxiliares y utilidades generales.
* `tests/` → Pruebas unitarias y de integración para asegurar la fiabilidad.
* `requirements.txt` → Dependencias necesarias para el backend.
* `README.md` → Documentación específica del backend.

## Tecnologías y Herramientas

* **Python 3.11+**
* **FastAPI** para la construcción de la API REST.
* **Pandas y Scikit-learn** para procesamiento y análisis de datos.
* **OpenAI API** para generación de análisis narrativo.
* **pytest** para pruebas unitarias.

## Instalación y Configuración

1. Crear entorno virtual:

```cmd
python -m venv venv
```

2. Activar entorno virtual:

```cmd
venv\Scripts\activate
```

3. Instalar dependencias:

```cmd
pip install -r requirements.txt
```

4. Ejecutar la API localmente:

```cmd
uvicorn main:app --reload
```

> [!IMPORTANT]
> Este entorno debe configurarse antes de cualquier desarrollo de funcionalidades para garantizar consistencia y reproducibilidad.

---

# frontend/README.md

# Frontend de SOCION

El **Frontend** de SOCION es responsable de la interacción con el usuario, ofreciendo una interfaz limpia, profesional y altamente interactiva para visualizar y manipular los resultados de las simulaciones.

## Objetivo

Permitir al usuario definir escenarios sociales, visualizar proyecciones y recibir análisis narrativos generados por la IA, manteniendo una experiencia de usuario profesional y consistente.

## Estructura Detallada

* `public/` → Archivos estáticos y recursos públicos.
* `src/components/` → Componentes reutilizables de UI.
* `src/pages/` → Páginas principales de la aplicación.
* `src/services/` → Funciones para comunicación con backend y gestión de datos.
* `src/App.js` → Componente principal que orquesta el flujo de la aplicación.
* `package.json` → Dependencias y configuración del proyecto.
* `README.md` → Documentación específica del frontend.

## Tecnologías y Herramientas

* **React 18+**
* **Tailwind CSS** para estilo moderno y consistente.
* **Plotly.js** para visualizaciones interactivas y gráficas avanzadas.
* **Axios** para comunicación eficiente con el backend.

## Instalación y Ejecución

1. Instalar dependencias:

```cmd
npm install
```

2. Ejecutar aplicación en modo desarrollo:

```cmd
npm start
```

3. Acceder a la interfaz mediante `http://localhost:3000`

> [!IMPORTANT]
> Mantener la separación entre lógica de presentación y servicios de datos es crítico para escalabilidad y mantenibilidad.

---

# data/README.md

# Datos de SOCION

La carpeta **data** contiene todos los datasets iniciales y de referencia que alimentan las simulaciones y análisis del proyecto SOCION.

## Objetivo

Garantizar la integridad, trazabilidad y claridad de los datos utilizados, proporcionando un repositorio centralizado y versionado de datasets.

## Contenido Detallado

* `world_data.csv` → Dataset inicial de referencia con variables sociales, económicas y ambientales.
* `README.md` → Documentación específica de la carpeta de datos.

## Buenas Prácticas

1. Mantener datasets limpios, normalizados y documentados.
2. Incluir siempre fuente y fecha de actualización de cada dataset.
3. No modificar archivos originales directamente; usar versiones controladas.
4. Documentar cualquier transformación o preprocesamiento realizado.

## Uso

Los datasets serán consumidos por el backend para ejecutar simulaciones y generar análisis narrativos, asegurando que los resultados sean reproducibles y consistentes.

> [!IMPORTANT]
> Toda modificación de datos debe ser rastreable mediante control de versiones para mantener profesionalidad y rigor en el proyecto.
