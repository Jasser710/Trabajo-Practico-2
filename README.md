# 🧑‍💻 Trabajo Práctico 2 - API REST con FastAPI

Este repositorio contiene el Trabajo Práctico 2 de la materia MLOps. El objetivo del proyecto es construir una API REST sencilla utilizando **FastAPI**, que permita crear y consultar usuarios.

## 📁 Estructura del proyecto

- `main.py`: Archivo principal donde se definen los endpoints de la API.
- `app/models.py`: Contiene el modelo `Usuario` que valida los datos mediante Pydantic.
- `README.md`: Instrucciones del proyecto.

## 🚀 Instrucciones para ejecutar el proyecto

### 1. Clonar el repositorio

git clone https://github.com/Jasser710/Trabajo-Practico-2.git

cd Trabajo-Practico-2

### 2. Crear y activar un entorno virtual

python -m venv venv

# Activar:
# En Windows:
venv\Scripts\activate
# En macOS/Linux:
source venv/bin/activate

### 3. Instalar librerías necesarias

pip install -r requirements.txt

### 4. Ejecutar el servidor

uvicorn main:app --reload

### 5. Probar los endpoints

Una vez iniciado el servidor, abrir en el navegador:

http://127.0.0.1:8000/docs

Desde esa interfaz podés probar los endpoints:

- `POST /user`: Crear un usuario (requiere nombre y email)
- `GET /user`: Obtener la lista de usuarios registrados

## 📌 Notas

- La aplicación utiliza una lista en memoria como base de datos simulada.
- Al reiniciar el servidor, los datos se pierden.

## ✍️ Autor

- Nombre: Jasser Palacios
- GitHub: https://github.com/Jasser710
