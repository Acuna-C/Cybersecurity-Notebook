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
```

---------------
### 🛠️ Insertar un registro
```
-- Insertar un solo registro
INSERT INTO usuarios (nombre, email, edad) 
VALUES ('Carlos', 'carlos@example.com', 25);

-- Insertar múltiples registros a la vez
INSERT INTO usuarios (nombre, email, edad) 
VALUES 
    ('Ana', 'ana@example.com', 30),
    ('Beatriz', 'beatriz@example.com', 22);
```
---------------
### 🛠️ Insertar un registro
```

---------------
-- Seleccionar todos los campos de todos los registros
SELECT * FROM usuarios;

-- Seleccionar columnas específicas
SELECT nombre, email FROM usuarios;

-- Filtrar por condiciones
SELECT * FROM usuarios WHERE edad >= 25;

-- Filtrar con operadores lógicos y ordenamiento
SELECT * FROM usuarios 
WHERE edad > 18 AND email LIKE '%@example.com'
ORDER BY edad DESC;
