# Taller 1 DCA - Luis Ángel Vivas

## Clase Main
Es la clase encargada de llamar a todos los metodos y clases para poder ejecurtar el programa.

### Metodos:
- **settings()**
Metodo utilicado para definir los parametros de size() que define el tamaño del lienzo.

- **setup()**
La función setup () se ejecuta una vez, cuando se inicia el programa. Se utiliza para definir las propiedades 
del entorno inicial.

- **draw()**
La función ejecuta continuamente las líneas de código contenidas dentro de su bloque hasta que se detiene 
el programa.

- **mousePRessed()**
La función se llama una vez después de cada vez que se presiona un botón del mouse.

- **mouseDragged()**
La función se llama una vez cada vez que se mueve el mouse mientras se presiona un botón del mouse.

- **mouseReleased()**
La función se llama cada vez que se suelta un botón del mouse.

- **mouseClicked()**
La función se llama después de presionar un botón del mouse y luego liberarlo.

- **mouseMoved()**
Se llama a la función cada vez que se mueve el mouse y no se presiona el botón del mouse.

- **keyPressed()**
La función se llama una vez cada vez que se presiona una tecla. La tecla presionada se almacena en la 
variable clave.

-------------------------------------------------------------------------------------------------------------------

## Clase Logica
Es la clase encargada de instanciar, llamar y operar las demás clases en las que se crearan objetos.

### Variables:
- **app**
Instancia de la libreria PApplet de Processing.

- **texto**
Es un String que va a contener el texto de donde se desprenderan las interacciones.

- **estrellas**
Un ArrayList de objetos de la clase Estrellas.

- **burbujas**
Un ArrayList de objetos de la clase Burbujas.

- **esferas**
Un ArrayList de objetos de la clase Esferas.

### Metodos:
- **getFrase(String)**
Esta función contiene al texto y lo analiza para desprender las interacciones.

- **pintar()**
Muestra todos los elementos en el lienzo.

- **arrastrar()**
Se encarga de todos los eventos del mouse que tengan que ver con la acción de arrastrar.

- **soltar()**
Se encarga de todos los eventos del mouse que tengan que ver con la acción de soltar despues de presionar click.

- **click()**
Se encarga de todos los eventos del mouse que tengan que ver con la acción de hacer click.

- **clickPresionado**
Se encarga de todos los eventos del mouse que tengan que ver con la acción de mantener presionado el click.

- **pasarMouse**
Se encarga de todos los eventos del mouse que tengan que ver con la acción de pasar el mouse en cierta area.

- **presionarTecla**
Se encarga de todos los eventos del teclado que tengan que ver con la acción de apresionar una tecla.

-------------------------------------------------------------------------------------------------------------------

## Clase Estrellas
Esta clase crea objetos que representan estrellas en el lienzo y aparecen en la parte superior del mismo.

### Variables:
- **x**
Es un int que representa una posición en el eje x del lienzo.

- **y**
Es un int que representa una posición en el eje y del lienzo.

- **tam**
Es un int que representa el tamaño del circulo que representara la estrella.

### Metodos:
- **pintar()**
Se encarga de hacer aparecer el objetos de tipo Estrellas en el lienzo.

-------------------------------------------------------------------------------------------------------------------

## Clase Rayo
Esta clase crea un objeto que representa un rayo en el lienzo despues de que el usuario haya presionado el click
durante 5 segundos.

### Variables:
- **x1**
Es un int que representa una posición en el eje x del lienzo y se usa en uno de los quad() que forma el relampago.

- **y1**
Es un int que representa una posición en el eje y del lienzo y se usa en uno de los quad() que forma el relampago.

- **x2**
Es un int que representa una posición en el eje x del lienzo y se usa en uno de los quad() que forma el relampago.

- **y2**
Es un int que representa una posición en el eje y del lienzo y se usa en uno de los quad() que forma el relampago.

- **xTri**
Es un int que representa una posición en el eje x del lienzo y se usa en un triangle() que forma el relampago.

- **yTri**
Es un int que representa una posición en el eje y del lienzo y se usa en un triangle() que forma el relampago.

### Metodos:
- **pintarRayo()**
Se encarga de hacer aparecer el objeto de tipo Rayo en el lienzo.

- **presMouseRayo()**
Se encarga del evento del mouse en el que el usuario debera mantener presionado el click.

-------------------------------------------------------------------------------------------------------------------

## Clase Cthulhu
Esta clase crea un objeto que representa a Cthulhu en el lienzo despues de que el usuario haya escrito su nombre
usando el teclado.

### Variables:
-**xCir**
Es un int que representa una posición en el eje x del lienzo y se usa en un ellipse() que forma a Cthulhu.

-**yCir**
Es un int que representa una posición en el eje y del lienzo y se usa en un ellipse() que forma a Cthulhu.

- **tam**
Es un int que representa el tamaño del circulo que será la cabeza de Cthulhu.

-**xArc**
Es un int que representa una posición en el eje x del lienzo y se usa en un arc() que forma a Cthulhu.

-**yArc**
Es un int que representa una posición en el eje y del lienzo y se usa en un arc() que forma a Cthulhu.

-**cArc**
Es un int que representa el ancho del arco y se usa en un arc() que forma a Cthulhu.

-**dArc**
Es un int que representa la altura del arco y se usa en un arc() que forma a Cthulhu.

-**xRect**
Es un int que representa una posición en el eje x del lienzo y se usa en un rect() que forma a Cthulhu.

-**yRect**
Es un int que representa una posición en el eje y del lienzo y se usa en un rect() que forma a Cthulhu.

-**letras[]**
Es un arreglo de char que contiene las letras que forman la palabra "Cthulhu".

-**valTecla**
Almacena un boolean que se usa en el metodo validarTecla(char).

### Metodos:
- **pintarCthulhu()**
Se encarga de hacer aparecer el objeto de tipo Cthulhu en el lienzo.

- **pintarFrase(char)**
Recibe como parametros las letras usadas para escribir la palabra "Cthulhu" y las pinta en el lienzo.

- **validarTecla(char)**
Valida si se escribe las teclas correctas para escribir la palabra "Cthulhu"-

- **getLetra(char)**
Retorna el char presionado por el usuario para que el programa lo valide.

-------------------------------------------------------------------------------------------------------------------




  