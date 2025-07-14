# 🎬 Recomendador de Películas según tu Estado de Ánimo

Este proyecto es una aplicación web que recomienda películas en función de cómo te sientes. Utiliza un modelo LLM (Groq via LangChain) para generar recomendaciones personalizadas en lenguaje natural. Las interacciones se almacenan en una base de datos PostgreSQL alojada en AWS.

---

## 🧠 ¿Cómo funciona?

1. El usuario introduce su estado de ánimo en la web.
2. Se envía una petición a una API construida con Flask.
3. El modelo LLM responde con una película adecuada.
4. La interacción (estado + recomendación) se guarda en la base de datos.

---

## 🚀 Tecnologías utilizadas

- **Python** (Flask, LangChain, dotenv)
- **Groq API** con modelo `mixtral-8x7b-32768`
- **PostgreSQL** (hosteado en **AWS RDS**)
- **HTML + JS** para el frontend
- **Docker** para contenerización
- **pgAdmin** para gestionar la base de datos
- **GitHub** para control de versiones

---


## ⚙️ Configuración

### 1. Clona el repositorio

```bash
git clone https://github.com/NereaLdA/LLM.git
cd tu-repo


### 2. Crea un archivo .env

GROQ_API_KEY=tu_clave_de_groq
DB_HOST=tu_host_aws
DB_PORT=5432
DB_NAME=nombre_de_tu_bbdd
DB_USER=tu_usuario
DB_PASSWORD=tu_contraseña


### 3. Instala las dependencias

pip install -r requirements.txt

### 4. Ejecuta con Docker

docker-compose up --build




