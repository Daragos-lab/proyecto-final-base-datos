# proyecto-final-base-datos

# Sistema de Gestión de Inventarios y Ventas (Tienda Express)

## 1. Integrantes del Equipo
- Cristian Andres Quiroga Manjarrez (CC. 1023623542 / cristianandresquiroga06@gmail.com)
- Freider Andres Murillo Palacios (TI. 1078856107 / freidermurillopalacios@gmail.com)
- Miguel Ángel Osorno Gutiérrez (CC. 1023634646 / miguelangelosorno84@gmail.com)

## 
2. Descripción del Negocio y Justificación
- Contexto general: La pequeña microempresa "Tienda Express" requiere automatizar el control de sus productos, ventas e inventario, reduciendo inconsistencias de stock y pérdidas operativas.
-Objetivo de la aplicación: Proveer una plataforma centralizada que permita gestionar categorías, productos, clientes y registrar pedidos/ventas asociadas con soporte multi-motor de base de datos en la nube

## 
3. Entidades Principales del Dominio
1. Categoría (`categoria`): Clasificación principal de los productos (ej. Abarrotes, Bebidas).(1:N)
2. Producto (`producto`): Artículos en inventario con información de precio, stock y categoría asociada.(1:N)
3. Cliente (`cliente`): Usuarios/compradores registrados en el sistema.(1:N)
4. Pedido (`pedido`): Registro de transacciones de compra realizadas por un cliente para un producto específico.(N:M)

## 
4. Matriz de Entornos y Conexiones
Motores y proveedores probados:
- SQLite: Archivo local (`mi_negocio.db`)
- MySQL: Instancia remota en Aiven.io
- PostgreSQL: Base de datos Serverless en Neon.tech
- PostgreSQL: Instancia en Render.com

##
5. Instrucciones de Ejecución
Comando de instalación de librerías:`pip install peewee psycopg2-binary pymysql`
Comando para ejecutar la aplicacion:`python app.py`
