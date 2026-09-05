
# 📊 Excel 

repositorio de funciones y herramientas avanzadas de **Microsoft Excel**! 

Este proyecto funciona como una guía de referencia rápida.

---


### 1. Funciones de Texto
* **Formato y Limpieza:**
  * `=MAYUSC(texto)` / `=MINUSC(texto)`: Convierte el texto a mayúsculas o minúsculas.
  * `=NOMPROPIO(texto)`: Convierte a formato de nombre propio (Primera Letra Mayúscula).
  * `=ESPACIOS(texto)`: Elimina espacios sobrantes al inicio, final o entre palabras.
  * `=CONCAT(texto1, [texto2], ...)`: Une varias cadenas de texto en una sola.
* **Extracción de Subcadenas:**
  * `=IZQUIERDA(texto; num_caracteres)`: Extrae caracteres desde el inicio.
  * `=DERECHA(texto; num_caracteres)`: Extrae caracteres desde el final.
  * `=EXTRAE(texto; posicion_inicial; num_caracteres)`: Extrae texto desde el centro.
* **Búsqueda y Tipo:**
  * `=LARGO(texto)`: Devuelve la cantidad total de caracteres.
  * `=ENCONTRAR(texto_buscado; dentro_del_texto; [pos_inicial])`: Ubica la posición exacta de un carácter (sensible a mayúsculas).
  * `=VALOR(texto)`: Convierte un texto con apariencia de número a un valor numérico real.

---

### 2. Funciones de Fecha y Tiempo
* **Partes de una fecha:** `=DIA(fecha)`, `=MES(fecha)`, `=AÑO(fecha)`, `=DIASEM(fecha; [tipo])`.
* **Operaciones y cálculo laboral:**
  * `=FECHA + NÚMERO`: Suma días del calendario a una fecha base.
  * `=DIA.LAB.INTL(fecha_inicial; dias; [fin_de_semana]; [dias_no_laborables])`: Suma días hábiles personalizados.
  * `=DIAS.LAB.INTL(fecha_inicial; fecha_final; [fin_de_semana]; [dias_no_laborables])`: Cuenta días laborables entre dos fechas.
* **Generación y formato:**
  * `=HOY()`: Devuelve la fecha actual dinámica.
  * `=FIN.MES(fecha_inicial; meses)`: Devuelve el último día del mes N meses antes o después.
  * `=TEXTO(valor; "formato")`: Convierte una fecha/número a formato texto personalizado (ej. `TEXTO(HOY(); "dddd, mmmm yyyy")`).

---

### 3. Lógicas y Funciones `.CONJUNTO`
* **`=SI.CONJUNTO(prueba_logica1; valor_si_verdadero1; ...)`**: Evalúa múltiples condiciones secuenciales sin necesidad de anidar varios `SI`.
* **`=SUMAR.SI.CONJUNTO(rango_suma; rango_criterio1; criterio1; ...)`**: Suma valores evaluando dos o más condiciones.
* **`=CONTAR.SI.CONJUNTO(rango_criterio1; criterio1; ...)`**: Cuenta filas que cumplen con múltiples criterios simultáneos.

---

### 4. Búsqueda y Matrices Dinámicas (Excel Moderno)
* **`=BUSCARX(valor_buscado; rango_busqueda; rango_devuelto; [si_no_se_encuentra])`**: Reemplazo moderno y flexible de `BUSCARV` (busca hacia la izquierda y derecha).
* **`=UNICOS(matriz)`**: Extrae valores sin duplicados de una lista.
* **`=ORDENAR(matriz; [indice_orden]; [criterio_orden])`**: Ordena un rango automáticamente.
* **`=FILTRAR(matriz; incluir; [si_vacio])`**: Filtra datos dinámicamente según un criterio lógico.
* **`=ELEGIRCOLS(matriz; num_col1; [num_col2]; ...)`**: Retorna únicamente las columnas especificadas de una tabla o matriz.

---

### 5. Validaciones y Formatos Condicionales
* **Validación de Datos:** Restringe la entrada en celdas mediante listas desplegables, números enteros, fechas o fórmulas personalizadas.
* **Formato Condicional:** Resalta celdas mediante reglas automáticas basadas en valores, fórmulas o barras de datos.
  * *Administración de Reglas:* `Inicio` $\rightarrow$ `Formato condicional` $\rightarrow$ `Administrar reglas` para editar la jerarquía o eliminar reglas existentes.

---

### 6. Tablas Dinámicas Avanzadas
* **Segmentación de Datos y Escalas de Tiempo:** Filtros visuales e interactivos para conectar múltiples tablas dinámicas a la vez.
* **Jerarquía de Fechas:** Agrupación automática por Años, Trimestres, Meses y Días al arrastrar campos de fecha.
* **Campos Calculados:** Agrega nuevas columnas personalizadas mediante fórmulas que operan sobre la **suma de los campos** existentes.
* **Elementos Calculados:** Agrega nuevas filas personalizadas dentro de una categoría específica de la tabla dinámica.
* **Mostrar Páginas de Filtro de Informes:** Genera automáticamente una pestaña/hoja individual en el libro por cada elemento de un filtro seleccionado.

---
