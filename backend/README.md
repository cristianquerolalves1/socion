

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

