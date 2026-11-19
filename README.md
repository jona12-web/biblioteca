# Sistema de Control de Biblioteca

Un sistema web ligero y funcional desarrollado para gestionar el registro, inventario y visualización de libros, utilizando **PHP**, **MySQL**, **HTML**, **CSS** y **JavaScript**.

![biblioteca](https://media.istockphoto.com/id/2162169941/es/foto/librer%C3%ADa.jpg?s=2048x2048&w=is&k=20&c=3Hz-55gIHhBslCoK9o9Q8iRWBZuxh32gNKCcJXwJCAA=)


## Estructura del Proyecto

El trabajo contiene 4 archivos principales:

 **`index.php`**: Página principal que muestra la interfaz visual. Contiene el formulario de registro y una tabla dinámica que lista el inventario actual de libros desde la base de datos.

  Este archivo es una de las partes más importantes del sistema, ya que permite que los usuarios interactúen directamente con la biblioteca digital. Desde aquí pueden visualizar los libros registrados, consultar su información y conocer cuáles se encuentran disponibles.

 **`guardar.php`**: Script backend encargado de recibir los datos del formulario por método POST, limpiar las variables contra inyecciones SQL básicas e insertar el nuevo libro en la base de datos.

  Su función es mantener actualizada la información del inventario, permitiendo almacenar los nuevos registros de manera organizada. Gracias a este archivo, los libros agregados quedan guardados en MySQL y pueden consultarse posteriormente desde la página principal.

**`script.js`**: Archivo de JavaScript del lado del cliente que realiza validaciones en tiempo real de los campos del formulario antes de enviarlos y maneja las alertas de éxito mediante parámetros en la URL.

  Este archivo ayuda a mejorar el funcionamiento de la página, evitando que se envíen formularios con información incompleta. También permite que la interacción con el sistema sea más sencilla y que el usuario reciba mensajes sobre las acciones realizadas.

 **`styles.css`**: Hoja de estilos encargada del diseño visual, utilizando variables CSS, diseño adaptable y estilos para las tablas y estados de los libros.

  Este archivo permite que el sistema tenga una presentación más atractiva y ordenada. Se encarga de establecer los colores, tamaños, espacios y estilos de los diferentes elementos, facilitando la navegación y mejorando la apariencia de la biblioteca digital.

---

## Requisitos Técnicos

* Servidor web con soporte para **PHP**
* Base de datos **MySQL** con una tabla llamada `libros` que contenga al menos los siguientes campos:
  * `id` (Entero, Auto-incremental, clave primaria)
  * `titulo` (Texto)
  * `autor` (Texto)
  * `isbn` (Texto)
  * `disponible` (Booleano o tinyInt para el estado)



## Estructura del Proyecto

El proyecto está compuesto por 4 archivos principales:

* **`index.php`**: Página principal que muestra la interfaz visual. Contiene el formulario de registro y una tabla dinámica que lista el inventario actual de libros desde la base de datos.
* **`guardar.php`**: Script backend encargado de recibir los datos del formulario por método POST, limpiar las variables contra inyecciones SQL básicas e insertar el nuevo libro en la base de datos.
* **`script.js`**: Archivo de JavaScript del lado del cliente que realiza validaciones en tiempo real de los campos del formulario antes de enviarlos y maneja las alertas de éxito mediante parámetros en la URL.
* **`styles.css`**: Hoja de estilos encargada del diseño visual, utilizando variables CSS, diseño adaptable y estilos para las tablas y estados de los libros.
