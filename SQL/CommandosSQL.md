# 🗄️ Guía de SQL

Guía de referencia rápida y práctica de **SQL** 
---

## 📌 1. Básico: Creación, Consultas y Manipulación de Datos

### 🛠️ Crear una Tabla
```sql
CREATE TABLE usuarios (
    id INT PRIMARY KEY AUTO_INCREMENT,
    nombre VARCHAR(50) NOT NULL,
    email VARCHAR(100) UNIQUE,
    edad INT,
    fecha_registro DATE DEFAULT CURRENT_DATE
);
