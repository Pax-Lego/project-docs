# 🍽️ Pax-Saporis

<p align="center">
  <img src="Documentation/logo.jgep" width="360"/>
  &nbsp
<p align="center">
  <strong>Descubre, crea y comparte recetas deliciosas.</strong><br>
  Una plataforma para explorar nuevas comidas, organizar planes de alimentación y compartir experiencias culinarias.
</p>

---

## 📖 Descripción

**Pax-Saporis** es una aplicación web diseñada para los amantes de la cocina.

La plataforma permite descubrir nuevas recetas, crear las propias, compartirlas con la comunidad y organizar planes de alimentación de manera sencilla e intuitiva.

Ya sea que busques una receta rápida para el almuerzo, una cena especial o inspiración para probar algo completamente nuevo, **Pax-Saporis** tiene un lugar para ti.

---

## ✨ Características

- 🍳 Crear y administrar recetas.
- 🌎 Compartir recetas con otros usuarios.
- 🔍 Buscar nuevas recetas.
- ❤️ Guardar tus recetas favoritas.
- 📅 Organizar planes de alimentación.
- 👤 Gestión de usuarios y autenticación.
- 📱 Interfaz moderna y responsive.

---

## 🚀 Estado del proyecto

🟢 **Estado:** Finalizado

---

## 🛠️ Tecnologías utilizadas

### Frontend

- ⚛️ React (Vite)
- 🎨 Tailwind CSS
- 🌐 Axios

### Backend

- 🐍 Django 4.2
- Django REST Framework
- django-cors-headers

### Base de datos

- 🗄️ SQLite (desarrollo)
- 🐘 PostgreSQL (producción)

### DevOps

- 🐳 Docker
- Docker Compose

### Herramientas

- Python 3.13
- Node.js
- npm
- virtualenv

---

# 📂 Estructura del proyecto

```text
Pax-Saporis/
│
├── project-frontend/     # Aplicación React
├── project-backend/      # API Django
├── docker-compose.yml
├── requirements.txt
└── README.md
```

---

# ⚙️ Instalación

## 1️⃣ Clonar el repositorio

```bash
git clone https://github.com/usuario/pax-saporis.git

cd pax-saporis
```

---

## 2️⃣ Configurar el Backend

Crear el entorno virtual

```bash
python -m venv venv
```

Activarlo

**Windows**

```bash
venv\Scripts\activate
```

**Linux / macOS**

```bash
source venv/bin/activate
```

Instalar dependencias

```bash
pip install -r requirements.txt
```

Aplicar migraciones

```bash
python manage.py migrate
```

Iniciar el servidor

```bash
python manage.py runserver
```

---

## 3️⃣ Configurar el Frontend

Entrar a la carpeta

```bash
cd project-frontend
```

Instalar dependencias

```bash
npm install
```

Ejecutar

```bash
npm run dev
```

El frontend estará disponible en

```
http://localhost:5173
```

---

# 🔒 Configuración importante

El frontend utiliza autenticación basada en cookies.

Antes de realizar solicitudes **POST**, obtiene automáticamente el token CSRF mediante:

```text
/api/auth/csrf/
```

Además, el backend debe permitir el origen del frontend durante el desarrollo:

```python
http://localhost:5173
```

mediante la configuración de **CORS**.

---

# 🐳 Docker

El proyecto incluye configuración para Docker y Docker Compose.

Desde la carpeta raíz puedes ejecutar:

```bash
docker compose up --build
```

---

# 👨‍💻 Desarrolladores

Proyecto desarrollado como parte de un proyecto académico.

---

# 📄 Licencia

Este proyecto se distribuye bajo la licencia MIT.
