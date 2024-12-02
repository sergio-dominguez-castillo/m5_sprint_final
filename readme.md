## Caso Shoes Tap – Sprint M5

Shoes Tap es un emprendimiento familiar que está en busca de poder lanzar su primera aplicación. Busca interactuar con usuarios que quieran comprar sus productos, básicamente una tienda en línea.
1. Primera Vista (View 1)
- Esta primera vista va a contener una lista de zapatos y zapatillas disponibles para la venta.
- Utiliza un LazyRow para mostrar los productos que conforman cada una de las listas. Cada producto debe estar contenido dentro de una Card que contenga la imagen y el precio.
- Recuerda aprovechar la segmentación del código para crear la Card una sola vez y no tener que repetir texto innecesariamente.
- Ten en cuenta que la cantidad de zapatos y zapatillas es un dato estático, es decir, no tiene un factor externo que lo afecte, por lo tanto, por esta vez su extensión está predefinida dentro del código.
----------
- En conclusión: La primera vista simplemente va a mostrar la cantidad de zapatos y zapatillas disponibles para la venta. Aprovecha los beneficios de LazyRow para mostrar ambas listas en su respectiva fila. También ten en cuenta que la cantidad de elementos que debe contener cada lista son estáticos, por ende, deben estar creados de manera manual (Por esta vez se permite el HardCoded solo en este punto).

2. Descripción del Producto (View 2)
- En este punto debes considerar que cada Card (Cada producto) debe tener la opción de ser clickable. De esta forma siempre que queramos ver el detalle de un producto se podrá hacer clic en su Card y se abrirá una nueva vista con su descripción.
- Importante para este punto tener en cuenta la implementación de navegación para ir de una vista a otra.
- La nueva vista debe incluir:
o Nombre del producto.
o Imagen del producto.
o Precio del producto.
o Botón de “Agregar al carrito”.
o Información extra: Tallas, colores, etc.
- Ten en cuenta que, al agregar un producto al carrito, este se almacena en dicha vista... quiere decir que se debe implementar una nueva lista que almacenará todo lo que el cliente va a comprar, independiente de si es una zapatilla o un zapato. Dato importante, el carrito de compra no debe borrarse al cerrar la aplicación o cambiar de vista, es decir, debe persistir mientras no concluya la compra. (DataStore te ayudará a cumplir con este objetivo).

3. Carrito de Compras (View 3)
- Esta vista debe mostrar todos los productos almacenados y, además debe darnos la opción de limpiar o eliminar uno a uno los productos.
- No olvides utilizar DataStore para que el carrito de productos persista aun cuando se cierre la aplicación.
- Esta nueva vista debe mostrar una lista de todos los productos seleccionados (LazyColumn te puede ayudar).
- La nueva Card debe mostrar el nombre, la imagen y cualquier otro dato relevante del producto, además del botón para eliminar. (No olvidar que ese botón simplemente elimina el producto, fuera debe existir uno general que limpie todo el carrito).

4. No olvides utilizar la arquitectura MVVM para mantener un orden en tu código. Además, puedes agregar carpetas como Components para fragmentar y reutilizar de mejor manera tu código.
5. Recuerda que el diseño no es un factor por evaluar, pero siempre se debe mantener coherencia con lo que estamos programando, al menos debe existir la preocupación de entregar un prototipo de aplicación profesional.
6. Una vez termines el proyecto, crea un nuevo repositorio en GitHub (Público) y sube a la plataforma el enlace por medio de un archivo .txt