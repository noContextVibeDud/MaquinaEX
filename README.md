# Máquina Expendedora - Proyecto Algoritmos 

Simulador de máquina expendedora desarrollado en Python con Programación Orientada a Objetos.

## Características

- **Catálogo** en matriz con coordenadas tipo ajedrez (A1, B2, ...).
- **Consulta de precios** actualizados desde GitHub.
- **Venta** con tarjetas prepagadas (hash SHA-256).
- **Restock** para actualizar existencia o cambiar productos (expansión dinámica de la matriz).
- **Reporte** en texto y gráficos (matplotlib).

## Requisitos

- Python 3.8 o superior
- pip (para instalar dependencias)

## Instalación y ejecución

1. Clonar o descargar el proyecto.
2. Crear un entorno virtual (opcional pero recomendado):
   ```bash
   python -m venv venv
   source venv/bin/activate   # Linux/Mac
   venv\Scripts\activate      # Windows
   ```
3. Instalar dependencias:
   ```bash
   pip install requests matplotlib
   ```
4. Ejecutar:
   ```bash
   python main.py
   ```

## Uso

Al iniciar, se muestra el catálogo y un prompt `>`.

- **Consultar precio**: escribir el código de 5 letras de un producto.
- **Vender**: presionar Enter, luego ingresar la coordenada y el número de tarjeta.
- **Restock**: escribir `RS` y seguir el menú.
- **Reporte**: escribir `RP` (genera `reporte.txt` y gráficos si matplotlib está instalado).

### Números de tarjeta válidos

- `1234567890`
- `9876543210`
- `1223334444`
- `4444333221`
- `1010101010`

## Estructura del código

- `main.py` - Punto de entrada.
- `catalogo.py` - Maneja la matriz y el archivo de inventario.
- `producto.py` - Modelo de producto.
- `tarjeta.py` - Modelo de tarjeta y hash.
- `repositorio.py` - Conexión con GitHub (precios y tarjetas).
- `venta.py` - Flujo de venta.
- `restock.py` - Operaciones de reposición.
- `reporte.py` - Generación de reportes y gráficos.

## Autoría

- 
- 

## Licencia

Proyecto académico – sin fines comerciales.
