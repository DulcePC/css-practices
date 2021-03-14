# css-practices
Here Im going to upload all my css practices, with tailwind.

# Flexbox
https://www.youtube.com/watch?v=_YUJ37FARrU
Al poner display flex hay dos ejex, Main-axis(horizontal), Cross-Axis(vertical)
Justify-content: no alinea elementos horizontalmente, alinea elmentos en el eje principal.

Main size -> main axis ( default: width)
Cross size -> cross axis (default: height)

Cross size:

1. Se ha definido el tamaño. ( tomara toda la altura del contenedor)

2. No se ha definido el tamaño y no se ha definido align-items o align-content (tomara la altura del item)

3.No se define un tamaño pero si se define alient-items o align-content diferente a stretch(si cumple con lo primero entonces se pondra del tamaño del item de lo contrario si lleva el stretch entonces sera del tamaño del contenedor.)

Main size:

1.espacio disponible: ( el espacio restante del contenedor), espacio ocupado: (el espacio ocupado por los items, a este se le suma el margin si los tienen).

2.Los margenes nunca se colapsan, osea nunca se reducen, los items si se reducen pero los margenes no.

3.El espacio puede ser negativo, es decir que los items suman mas que el tamaño del contenedor.

--------------------

-Flex-basis: es igual al width del item. width:120px === flex-basis:120px; ( recuerda que es width si el main esta en horizontal, de lo contrario si esta en vertical cambiara a height)

-Flex-grow: como va a crecer un elemento, para ocupar el espacio disponible

-Flex-shrink: (por defecto todos los items tiene esta propiedad) encojes el item hasta que todo el espacio sobrante llegue a 0

flex = ( default = 0 1 auto) = flex es esto: 
flex-grow
flex-shrink
flex-basis

flex-none = flex 0 0 auto;
flex-auto = 1 1 auto; 