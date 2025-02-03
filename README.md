# Tarea 12 Odoo
## Apartado 1
`Como mencionamos en clase, aunque no es recomendable, en ocasiones puede ser
necesario crear tablas ajenas a Odoo dentro de su base de datos (integración con
sistemas externos, almacenamiento de históricos, datos temporales…). Mediante la
herramienta PgAdmin u otro método que estimes oportuno, elabora y ejecuta una
sentencia que cree una tabla llamada “EmpresasFCT“con los siguientes campos:`
- Creamos una nueva tabla y añadimos las columnas

![IMG1](imgs/img1.png)

## Apartado 2

`Inserta 5 registros inventados en la tabla a través de una sentencia SQL.`

- Creamos la siguiente sentencia SQL para insertar los registros

![IMG2](imgs/img2.png)

## Apartado 3

`Realiza una consulta donde se muestren todos los datos de la tabla EmpresasFCT
ordenados por fechaContacto, de modo que en la primera la salga el que tenga la
fecha más reciente.`

```sql
SELECT * FROM public."EmpresasFCT"  
ORDER BY "fechaContacto" DESC;
```

![IMG3](imgs/img3.png)

## Apartado 4
`Utilizando las tablas de odoo, obtén un listado de empresas proveedoras, que han
emitido algún reembolso (facturas recticativas de proveedor)`



