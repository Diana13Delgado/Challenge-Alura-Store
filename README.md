<h1>Challenge Alura Sotore</h1>


Durante este desafío de análisis de datos, ayudamos al Sr. Juan a tomar una decisión estratégica: **¿qué tienda de la cadena Alura Store debería vender para comenzar un nuevo emprendimiento?**

Para responder a esta pregunta, analizamos datos de ventas, rendimiento, reseñas de clientes y costos logísticos de **4 tiendas diferentes**.


---

## Objetivo del Proyecto

Determinar la tienda menos eficiente a partir de datos de ventas, reseñas y costos.
---
## Archivos Incluidos

url = "https://raw.githubusercontent.com/alura-es-cursos/challenge1-data-science-latam/refs/heads/main/base-de-datos-challenge1-latam/tienda_1%20.csv"
url2 = "https://raw.githubusercontent.com/alura-es-cursos/challenge1-data-science-latam/refs/heads/main/base-de-datos-challenge1-latam/tienda_2.csv"
url3 = "https://raw.githubusercontent.com/alura-es-cursos/challenge1-data-science-latam/refs/heads/main/base-de-datos-challenge1-latam/tienda_3.csv"
url4 = "https://raw.githubusercontent.com/alura-es-cursos/challenge1-data-science-latam/refs/heads/main/base-de-datos-challenge1-latam/tienda_4.csv"

tienda = pd.read_csv(url)
tienda2 = pd.read_csv(url2)
tienda3 = pd.read_csv(url3)
tienda4 = pd.read_csv(url4)

**Cada archivo contiene:**
- "Producto" → Nombre del producto vendido.
- "Categoría del Producto" → Clasificación del producto.
- "Precio" → Valor de la venta.
- "Calificación" → Puntuación otorgada por el cliente.
- "Costo de envío" → Valor del envío.
- "Fecha de compra" → El dia en que se hizo la compra.
- "Vendedor" → Persona que realizo la venta
- "Lugar de compra" → Lugar en donde se realizo la compra.
- "Método de pago" → La forma en que se pago el producto.
- "Cantidad de cuotas" →  La cantidad de pagos que se hicieron para comprar el producto.
- "lat y long " →  Punto exacto en donde se realizo la compra.

- ## 🛠️ Instalación
- 1.Clona este repositorio o descarga el notebook AluraStoreLatam.ipynb.
- 2.Ejecuta cada celda en orden para realizar el análisis completo.
- 3.Asegúrate de tener conexión a internet, ya que los datos se cargan desde URLs

## 🛠 Tecnologías utilizadas
- **Python 3**
- **Pandas** para análisis de datos
- **Matplotlib y Numpy** para visualizaciones
- **Jupyter Notebook**

- 
## 📁 Análisis Realizados

1. ### 💰 Ingreso Total por Tienda  
   Se calcularon los ingresos sumando los valores de la columna **Precio** en los archivos CSV de cada tienda.

2. ### 📦 Ventas por Categoría  
   Agrupamos los productos vendidos por categoría y contamos la cantidad vendida para identificar las categorías más populares en cada tienda.

3. ### ⭐ Calificaciones Promedio  
   Calculamos el promedio de reseñas de los clientes para cada tienda, con el fin de evaluar la **satisfacción del cliente**.

4. ### 🔝 Productos Más y Menos Vendidos  
   Identificamos los productos más populares (y los menos vendidos) de cada tienda. Los resultados fueron visualizados gráficamente.

5. ### 🚚 Costo Promedio de Envío  
   Analizamos el gasto logístico promedio por tienda, calculando el valor medio de la columna de **costo de envío**.


- ## 📈 Resultados finales

### 💰 Ingresos totales
| Tienda  | Facturación ($) |
|---------|-----------------|
| Tienda 1 | 1,150,880,400.00 |
| Tienda 2 | 1,116,343,500.00 |
| Tienda 3 | 1,098,019,600.00 |
| Tienda 4 | 1,038,375,700.00 |
<img width="691" height="470" alt="image" src="https://github.com/user-attachments/assets/58957b64-c7fd-4acc-bee7-e20e89bf1655" />

---

### 🏷 Categorías más y menos vendidas

**Ejemplo Tienda 1:**
- Más vendida: **Muebles** (465)
- Menos vendida: **Artículos para el hogar** (171)

*(Ver el archivo colab para la lista de todas las tiendas)*
<img width="1189" height="590" alt="image" src="https://github.com/user-attachments/assets/49b6d952-49fc-4fff-b04f-2ad2ac859b23" />

---

### ⭐ Calificación promedio por tienda
| Tienda  | Calificación promedio |
|---------|-----------------------|
| Tienda 1 | 3.98 |
| Tienda 2 | 4.04 |
| Tienda 3 | 4.05 |
| Tienda 4 | 4.00 |

---

### 🛒 Producto más y menos vendido
- **Tienda 1:** Más vendido → Microondas (60) | Menos vendido → Celular ABXY (33)  
- **Tienda 2:** Más vendido → Iniciando en programación (65) | Menos vendido → Juego de mesa (32)  
- **Tienda 3:** Más vendido → Kit de bancas (57) | Menos vendido → Bloques de construcción (35)  
- **Tienda 4:** Más vendido → Cama box (62) | Menos vendido → Guitarra eléctrica (33)  

---

### 🚚 Costo de envío promedio
| Tienda  | Costo envío promedio ($) |
|---------|--------------------------|
| Tienda 1 | 26,018.61 |
| Tienda 2 | 25,216.24 |
| Tienda 3 | 24,805.68 |
| Tienda 4 | 23,459.46 |
<img width="790" height="590" alt="image" src="https://github.com/user-attachments/assets/8c032db7-c750-41de-adc4-9a31321e27ea" />

---

## 📌 Conclusión
Con base en las métricas de ingresos, satisfacción del cliente y costos de operación, la **Tienda 4** presenta menor facturación y costo de envío, por lo que podría ser la mejor opción para vender.

---

## 📦 Librerías usadas
- "pandas"
- "matplotlib"

