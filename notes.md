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
