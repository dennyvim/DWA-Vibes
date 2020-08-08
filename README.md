# DWA-Vibes


## Descripción de la aplicación

Para el desarrollo de esta aplicación se requiere el servicio de bases de datos para el almacenamiento y mejor desempeño de la aplicación ya que constantemente se agregar nuevas entradas al catálogo por lo que es necesario una consulta a una base de datos para traer la información de las mismas, además de los productos y la cantidad que quedan en inventario de los mismos para la personalización de los mismos.

Para el catalogo debemos recibir entonces la siguiente información
```json
{
    id
    Nombre_Ancheta
    Descripcion
    productos
    {
    } 
    precio
}

Esto por toda la cantidad de productos que estén en la base de datos, esto por un método GET

Ahora para la publicación de las anchetas personalizadas, es decir, se debe hacer un GET de todos los productos disponibles pero al hacer un post el campo productos será diferente.

Otro servicio a consumir será el de la pasarela de pagos de Bancolombia llamado Wompi, donde entonces se hará consumo de su API como servicio externo para el cobro de los mismos, además en la base de datos debe estar almancenado todos los datos de las transacciones hechas como otra entidad.

## Bibliografia

Construcción de árbol de problemas:
https://legalidadpormexico.org/mcl/modulo1/arboldeproblemas.html

Construcción de Lean Canvas:
https://www.oleoshop.com/blog/que-es-el-lean-canvas-y-como-implementarlo

Referentes:
https://www.frontendmentor.io/challenges

