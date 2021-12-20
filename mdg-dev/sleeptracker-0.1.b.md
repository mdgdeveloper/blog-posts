La siguiente iteración del desarrollo de la app se centra en el ciclo de inserción y finalización de una entrada. 

## Inserción
### Funciones
```javascript
insert(date);
// Devuelve la entrada insertada.
// Devuelve error en caso de no poder realizar la operacion.
```
Lanzada al presionar el boton de nueva entrada, automaticamente genera una entrada con la fecha y la hora del instante de la inserción.

Para evitar duplicados, comprueba que en los últimos 7 eventos no haya ninguna inserción que se haya realizado en las últimas 12 horas: en caso de serlo, lanzaría un error. 

Actualización: He visto que era bastante más sencillo gestionar esto desde el frontend. Así, si hay un evento activo, directamente el usuario no puede insertar ningún nuevo evento. 

Si todo está correcto, lanza una nueva inserción. 


## Presentacion 
Esta fase muestra disponibles aquellos botones que, dados los datos obtenidos, pueden ser usados por el usuario:


- [ ] En caso de no haber entradas que tengan que cerrarse, el link new sleep está activo.

- [ ] En caso de haber una entrada activa, el link New Sleep está desactivado y aparece la opción de cerrar el ciclo


## Valoración
La última fase del ciclo de inserción es la valoración y cierre de la entrada abierta.

Esta valoración es la que indica nuestra calidad percibida del sueño y nos va a permitir realizar análisis de tendencias en el dashboard de la aplicación.

La forma de valorar nuestra calidad de sueño es mediante estrellas de 1 a 5. 

Una vez el valor es insertado, se habilita el botón de enviar valoración y, con ello, se lanza la última parte del proceso.

## Cierre 
Cuando ya disponemos de todos los datos necesarios: fecha de inicio, fecha de fin y valoración del sueño, la entrada se puede cerrar.

Esto se realiza llamándo a la API y actualizando la entrada al mismo tiempo que se vuelve a habilitar la opción de crear una nueva entrada. 

