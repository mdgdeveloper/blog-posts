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

Si todo está correcto, lanza una nueva inserción. 


## Presentacion 
Esta fase muestra disponibles aquellos botones que, dados los datos obtenidos, pueden ser usados por el usuario:

```javascript
getLast12();
// Devuelve la entrada de las ultimas 12 horas
// Devuelve FALSE en caso de no haber ninguna.
```

- [ ] En caso de no haber entradas de las ultimas 12 horas, el link new sleep está activo.

- [ ] En caso de haber entradas en las ultimas 12 horas, el link New Sleep está desactivado y aparece la opción de cerrar el ciclo
### Funciones




```javascript
getLast(date)
```





La función getLast(date) devuelve la entrada pendiente en las últimas 24 horas o false en caso de no haber ninguna. 
