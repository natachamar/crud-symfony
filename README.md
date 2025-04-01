# 🚀 CRUD con Symfony

Este proyecto es un sistema CRUD desarrollado con **Symfony** y utiliza **AdminKit** para la interfaz de administración.

## 📂 Requisitos

Antes de comenzar, asegúrate de tener instalados los siguientes programas:

- **PHP** (>= 8.1)
- **Composer**
- **Symfony CLI** (Opcional pero recomendado)
- **Node.js** y **npm** (para gestionar assets)
- **MySQL** o cualquier base de datos compatible con Doctrine

---

## 📥 Instalación

Sigue estos pasos para clonar e instalar el proyecto:

### 1️⃣ Clona el repositorio

git clone https://github.com/natachamar/crud-symfony.git

cd crud-symfony

### 2️⃣ Instala las dependencias de PHP

composer install

### 3️⃣ Configura las variables de entorno

Copia el archivo .env.example y renómbralo como .env:

cp .env.example .env

Luego edita el archivo .env y configura los datos de tu base de datos:

DATABASE_URL="mysql://root:@127.0.0.1:3306/venta-productos?serverVersion=8.0"

### 4️⃣ Crea la base de datos y ejecuta las migraciones

php bin/console doctrine:database:create

php bin/console doctrine:migrations:migrate

### 5️⃣ Instala las dependencias de Node.js y genera los assets

npm install

npm run build

### ▶️ Ejecutar el servidor

symfony serve


