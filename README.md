# DWA-Vibes

## Estado del arte

Al día de hoy múltiples tiendas de regalos tales como Almara, Juan Regala, Cielo mío regalos con amor, Amada entrega, entre otros, ofrecen el servicio de venta a través de su sitio web, sin embargo sólo incluyen productos estándar, es decir, ofrecer un catálogo limitado, donde el cliente puede seleccionar el sabor de algunos productos, personalizar el mensaje que acompaña el regalo y algunas permiten hacer adiciones, pero no se pueden realizar cambios en función de la composición o el contenido de los mismos. Otras, como Rincón de Ilusiones, emplean otras plataformas como Rappi para la venta de sus productos, sin embargo, allí tampoco es posible personalizar los regalos. Así pues, lo que se busca con el desarrollo de este aplicativo web es darle la posibilidad al usuario tanto de comprar un producto de catálogo como uno totalmente personalizado, donde él puede armar desde cero su detalle, seleccionando uno a uno los productos que quieren que lo compongan, la forma del empaque, los colores, temáticas y mensaje, esto con el fin de entregar regalos únicos y que se acoplen perfectamente a las necesidades, gustos y presupuesto de los clientes. 
[Almara:] (https://www.almara.com.co/tienda/)
[Juan regala:] (https://juanregala.com.co/medellin/)
[Cielo mío regalos con amor:] (http://www.cielomioconamor.com/)
[Amada entrega:] (https://www.amadaentrega.com/)
[Rincón de ilusiones:] (https://rincondeilusiones.com/)


## Objetivo General 

Desarrollar una aplicación web para una tienda de regalos que permita la visualización y compra de sus productos de catálogo además de personalizar los mismos y ofrecerle al cliente una visualización integral de todo el proceso.


## Objetivos específicos

* Desarrollar la sección de catálogo donde se muestren los productos predefinidos 
* Desarrollar la sección de personalizar donde el cliente pueda elegir los productos de su regalo personalizado
* Hacer integración con la pasarela de pagos Wompi para que el cobro del regalo



## Mockups de la aplicación

Para los mockups de la aplicación se utilizo Figma como herramienta facilitadora, se agrega el link entonces para redigirse allí a mirar los diseños.

Home:

https://www.figma.com/file/Lz323CGqfrevaSyeBzauWp/Vibes_Detalles?node-id=37%3A1

Catalogo:

https://www.figma.com/file/Lz323CGqfrevaSyeBzauWp/Vibes_Detalles?node-id=69%3A82

Personalizar:

https://www.figma.com/file/Lz323CGqfrevaSyeBzauWp/Vibes_Detalles?node-id=69%3A84


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


