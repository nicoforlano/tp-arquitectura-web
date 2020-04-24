# Trabajo Práctico - Arquitectura Web
Este repositorio contiene el código del trabajo práctico realizado para la materia Arquitectura Web - Universidad de Palermo. El negocio seleccionado es una API REST desarrollada en NodeJS que expone endpoints para gestionar las operaciones básicas CRUD de productos de supermercado para una tienda online y otros adicionales que permiten obtener datos relevantes.  
MongoDB ha sido la tecnología NoSQL seleccionada para almacenar estos recursos.

## Integrantes del Grupo
- Hugo Centurión
- Nicolás Forlano

## Instalación
### Requerimientos

## Endpoints
- **Productos**
  - **_Obtener Productos_**
    - **Verbo HTTP**: GET
    - **Endpoint**: /productos
    - **Parámetros**:
      - _limit_ -> Cantidad de resultados.
      - _offset_ -> Comenzando desde.
      - _query_ -> Filtro de búsqueda por nombre del producto.
      - _precio-desde_ -> Precio mínimo del producto.
      - _precio-hasta_ -> Precio máximo del producto.
  - **_Obtener Producto_**
    - **Verbo HTTP**: GET
    - **Endpoint**: /productos/{idProducto}
    - **Códigos de Error Posibles**:
      - _**400** BAD REQUEST_
      - _**404** NOT FOUND_
  - **_Crear Producto_**
    - **Verbo HTTP**: POST
    - **Endpoint**: /productos
    - **Códigos de Error Posibles**:
      - _**400** BAD REQUEST_
  - **_Modificar Producto_**
    - **Verbo HTTP**: PUT
    - **Endpoint**: /productos
    - **Códigos de Error Posibles**:
      - _**400** BAD REQUEST_
  - **_Eliminar Producto_**
    - **Verbo HTTP**: DELETE
    - **Endpoint**: /productos/{idProducto}
    - **Códigos de Error Posibles**:
      - _**400** BAD REQUEST_
      - _**404** NOT FOUND_
- **Categorías**
  - **_Obtener Categorías_**
    - **Verbo HTTP**: GET
    - **Endpoint**: /categorias
    - **Parámetros**:
      - _limit_ -> Cantidad de resultados
      - _offset_ -> Comenzando desde
      - _query_ -> Filtro de búsqueda por nombre de la categoría
  - **_Obtener Categoría_**
    - **Verbo HTTP**: GET
    - **Endpoint**: /categorias/{idCategoria}
    - **Códigos de Error Posibles**:
      - _**400** BAD REQUEST_
      - _**404** NOT FOUND_
  - **_Crear Categoría_**
    - **Verbo HTTP**: POST
    - **Endpoint**: /categorias
    - **Códigos de Error Posibles**:
      - _**400** BAD REQUEST_
  - **_Modificar Categoría_**
    - **Verbo HTTP**: PUT
    - **Endpoint**: /categorias
    - **Códigos de Error Posibles**:
      - _**400** BAD REQUEST_
  - **_Eliminar Categoría_**
    - **Verbo HTTP**: DELETE
    - **Endpoint**: /categorias/{idCategorias}
    - **Códigos de Error Posibles**:
      - _**400** BAD REQUEST_
      - _**404** NOT FOUND_
  - **_Obtener Productos de una Categoría_**
    - **Verbo HTTP**: GET
    - **Endpoint**: /categorias/{idCategoria}/productos
    - **Códigos de Error Posibles**:
      - _**400** BAD REQUEST_
      - _**404** NOT FOUND_
- **Usuarios**
  - **_Obtener Usuarios_**
    - **Verbo HTTP**: GET
    - **Endpoint**: /usuarios
    - **Parámetros**:
      - _limit_ -> Cantidad de resultados
      - _offset_ -> Comenzando desde
      - _query_ -> Filtro de busqueda por nombre de usuario
  - **_Obtener Usuario_**
    - **Verbo HTTP**: GET
    - **Endpoint**: /usuarios/{idUsuario}
    - **Códigos de Error Posibles**:
      - _**400** BAD REQUEST_
      - _**404** NOT FOUND_
  - **_Crear Usuario_**
    - **Verbo HTTP**: POST
    - **Endpoint**: /usuarios
    - **Códigos de Error Posibles**:
      - _**400** BAD REQUEST_
  - **_Modificar Usuario_**
    - **Verbo HTTP**: PUT
    - **Endpoint**: /usuarios
    - **Códigos de Error Posibles**:
      - _**400** BAD REQUEST_
  - **_Eliminar Usuario_**
    - **Verbo HTTP**: DELETE
    - **Endpoint**: /usuarios/{idUsuario}
    - **Códigos de Error Posibles**:
      - _**400** BAD REQUEST_
      - _**404** NOT FOUND_
- **Pedidos**
  - **_Obtener Pedidos_**
    - **Verbo HTTP**: GET
    - **Endpoint**: /pedidos
    - **Parámetros**:
      - _limit_ -> Cantidad de resultados.
      - _offset_ -> Comenzando desde.
      - _query_ -> Filtro de busqueda por nombre de los productos.
      - _importe-desde_ -> Importe mínimo del pedido.
      - _importe-hasta_ -> Importe máximo del pedido.
      - _fecha-desde_ -> Fecha desde la cual se buscan pedidos.
      - _fecha-hasta_ -> Fecha hasta la cual se buscan pedidos.
  - **_Obtener Pedido_**
    - **Verbo HTTP**: GET
    - **Endpoint**: /pedidos/{idPedido}
    - **Códigos de Error Posibles**:
      - _**400** BAD REQUEST_
      - _**404** NOT FOUND_
  - **_Crear Pedido_**
    - **Verbo HTTP**: POST
    - **Endpoint**: /pedido
    - **Códigos de Error Posibles**:
      - _**400** BAD REQUEST_
  - **_Modificar Pedido_**
    - **Verbo HTTP**: PUT
    - **Endpoint**: /pedidos
    - **Códigos de Error Posibles**:
      - _**400** BAD REQUEST_
  - **_Cancelar Pedido_**
    - **Verbo HTTP**: DELETE
    - **Endpoint**: /pedidos/{idPedido}
    - **Códigos de Error Posibles**:
      - _**400** BAD REQUEST_
      - _**404** NOT FOUND_