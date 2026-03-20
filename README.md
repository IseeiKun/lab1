Alumno: Justin Steven Franco Martinez
# Sistema Web de Control de Ventas

## Situación problemática

En la ciudad de San Miguel, muchos pequeños negocios no cuentan con un sistema digital para registrar sus ventas, lo que provoca desorden, pérdida de información y errores en los cálculos.

## Sectores beneficiados

- Pequeños negocios
- Emprendedores
- Tiendas locales

## Solución propuesta

Se desarrolló una aplicación web utilizando Vue.js que permite registrar productos vendidos, calcular totales y llevar control de ventas de forma sencilla.

## Funcionalidades

- Registro de productos
- Ingreso de cantidad y precio
- Cálculo automático del total
- Visualización de ventas
- Eliminación de registros
- Validación de datos
¿Qué es Vue.js y cuál es su función en la página web?

Vue.js es un framework de JavaScript que permite crear interfaces interactivas de forma sencilla y organizada. Su función dentro de la página web desarrollada es manejar la lógica de la aplicación, actualizar automáticamente la interfaz cuando cambian los datos y facilitar la interacción del usuario con el sistema sin necesidad de recargar la página.

Variables reactivas utilizadas

En la aplicación se utilizaron las siguientes variables reactivas:

producto: almacena el nombre del producto ingresado por el usuario.

cantidad: guarda la cantidad del producto vendido.

precio: almacena el precio del producto.

ventas: es un arreglo donde se guardan todas las ventas registradas.

error: guarda mensajes de error cuando los datos ingresados no son válidos.

Estas variables permiten que la interfaz se actualice automáticamente cada vez que cambian.

Diferencia entre v-bind y v-model

v-model: se utiliza para enlazar datos de los inputs con las variables reactivas. Permite que lo que el usuario escribe se guarde automáticamente en el sistema.

v-bind: se utiliza para enlazar atributos HTML con datos dinámicos. Por ejemplo, se usa para asignar valores dinámicos como estilos o claves (:key).

En resumen:

v-model → conecta inputs con datos

v-bind → conecta atributos HTML con datos

Ejemplo de evento utilizado

Un ejemplo de evento utilizado es:

@click="agregarVenta"

Este evento se ejecuta cuando el usuario hace clic en el botón "Agregar", permitiendo registrar una nueva venta en el sistema.

uso de v-for

La directiva v-for se utilizó para recorrer la lista de ventas y mostrarlas en pantalla dinámicamente.

Permite que cada vez que se agrega una nueva venta, esta aparezca automáticamente en la lista sin necesidad de recargar la página.

Uso de v-if

La directiva v-if se utilizó para mostrar mensajes de error solo cuando existen problemas en los datos ingresados.

Ejemplo:

Cuando los campos están vacíos

Cuando los valores son incorrectos

Esto evita mostrar mensajes innecesarios y mejora la experiencia del usuario.

🔹 Validación de datos

La validación se realiza dentro del método agregarVenta(), donde se verifica:

Que los campos no estén vacíos

Que los valores sean mayores a cero

Si hay un error, se muestra un mensaje al usuario y no se guarda la venta.
