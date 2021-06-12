# Curso de asincronismo con JavaScript

## Definición y estructura de un  callback

### ¿Qué es un callback?

Es una función que al crearla le pasamos como parametro una segunda función, y de esta forma cuando hacemos alguna petición asincrona, esta se ejecuta despues de este llamado.

Por convención, esta función que se manda por parametro se va a llamar callback

## XMLHttpRequest

Es un objeto de JS que nos permite hacer peticiones a algun servicio en la nube (API's)

### XMLHttpRequest.readyState

La propiedad readyState retorna el estado en el que está la petición XMLHttp. los estados son los siguientes

| value | state | description |
|-------|-------|-------------|
| 0 | UNSENT | El cliente ha sido creado, no se ha llamado al metodo `open()`. |
|1 | OPENED | `open()` has been called.|
|2	| HEADERS_RECEIVED	| send() has been called, and headers and status are available.|
|3 | LOADING | Downloading; responseText holds partial data.|
|4 | DONE | The operation is complete.|

> Un standard de los callbacks dentro de node que el primero valor del callback es el error y el segundo es la información que se desencadena.

## Promesas

Vienen del objeto Promise, es algo que va a suceder pero no se sabe cuando, puede ser ahora, en el futuro o nunca.

¿Para qué nos sirve xhttp.status === 200?

* Comprobar que el estado de la petición xhttps es igual a 200

¿Cual es el método recomendando por la comunidad para manejar asincronismo en JavaScript?

* async/await

¿Para qué utilizamos `JSON.parse(xhttp.responseText)`?

* convertir una respuesta en texto a un objeto inmutable

¿La recomendación de la comunidad para anidar callbacks es?

* usar un maximo de 3 callbacks