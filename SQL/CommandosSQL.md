#  Guía de SQL

Guía de referencia rápida y práctica de **SQL** 
---

##  1. Básico: Creación, Consultas y Manipulación de Datos

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

### 🛠️ Insertar un registro
```sql
-- Insertar un solo registro
INSERT INTO usuarios (nombre, email, edad) 
VALUES ('Carlos', 'carlos@example.com', 25);

-- Insertar múltiples registros a la vez
INSERT INTO usuarios (nombre, email, edad) 
VALUES 
    ('Ana', 'ana@example.com', 30),
    ('Beatriz', 'beatriz@example.com', 22);
```

### 🛠️ Consultas
```sql

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

```

### 🛠️ Actualizar Registro
```sql

UPDATE usuarios 
SET edad = 26 
WHERE id = 1;

```

### 🛠️ ELIMINAR UN DATO 
```sql

-- Borrar un registro específico por su clave primaria
DELETE FROM usuarios WHERE id = 2;

-- Borrar múltiples registros bajo una condición
DELETE FROM usuarios WHERE edad < 18;

```

### 🛠️ Cruce de Información (JOINs)
```sql

-- INNER JOIN: Devuelve solo los registros que coinciden en ambas tablas
SELECT clientes.nombre, pedidos.producto, pedidos.monto
FROM clientes
INNER JOIN pedidos ON clientes.id = pedidos.cliente_id;

-- LEFT JOIN: Devuelve todos los clientes, tengan o no un pedido asociado
SELECT clientes.nombre, pedidos.producto
FROM clientes
LEFT JOIN pedidos ON clientes.id = pedidos.cliente_id;

-- RIGHT JOIN: Devuelve todos los pedidos, incluso si no tienen un cliente válido asociado
SELECT clientes.nombre, pedidos.producto
FROM clientes
RIGHT JOIN pedidos ON clientes.id = pedidos.cliente_id;


```

### 🛠️ Consultar y Sustraer Datos entre Múltiples Bases de Datos
```sql

SELECT 
    v.id_venta,
    v.fecha,
    e.nombre AS nombre_empleado
FROM bd_ventas.ventas AS v
INNER JOIN bd_rrhh.empleados AS e 
    ON v.id_empleado = e.id_empleado;
