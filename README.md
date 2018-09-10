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
- **xCir**
Es un int que representa una posición en el eje x del lienzo y se usa en un ellipse() que forma a Cthulhu.

- **yCir**
Es un int que representa una posición en el eje y del lienzo y se usa en un ellipse() que forma a Cthulhu.

- **tam**
Es un int que representa el tamaño del circulo que será la cabeza de Cthulhu.

- **xArc**
Es un int que representa una posición en el eje x del lienzo y se usa en un arc() que forma a Cthulhu.

- **yArc**
Es un int que representa una posición en el eje y del lienzo y se usa en un arc() que forma a Cthulhu.

- **cArc**
Es un int que representa el ancho del arco y se usa en un arc() que forma a Cthulhu.

- **dArc**
Es un int que representa la altura del arco y se usa en un arc() que forma a Cthulhu.

- **xRect**
Es un int que representa una posición en el eje x del lienzo y se usa en un rect() que forma a Cthulhu.

- **yRect**
Es un int que representa una posición en el eje y del lienzo y se usa en un rect() que forma a Cthulhu.

- **letras[]**
Es un arreglo de char que contiene las letras que forman la palabra "Cthulhu".

- **valTecla**
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

## Clase Tentaculo
Esta clase crea un objeto que representa a un tentaculo de Cthulhu en el lienzo despues de que el usuario haya 
pasado el mouse por cierta zona del lienzo.

### Variables:
- **xCir**
Es un int que representa una posición en el eje x del lienzo y se usa en un ellipse() que forma una roca.

- **yCir**
Es un int que representa una posición en el eje y del lienzo y se usa en un ellipse() que forma una roca.

- **xCirT**
Es un int que representa una posición en el eje x del lienzo y se usa en un ellipse() que forma al tentaculo 
de Cthulhu.

- **yCirT**
Es un int que representa una posición en el eje y del lienzo y se usa en un ellipse() que forma al tentaculo 
de Cthulhu.

- **tam**
Es un int que representa el tamaño del circulo que representara una roca.

- **tamT**
Es un int que representa el tamaño del circulo que representara una ventosa del tentaculo de Cthulhu.

- **xTrian**
Es un int que representa una posición en el eje x del lienzo y se usa en un triangle() que forma al tentaculo 
de Cthulhu.

- **yTrian**
Es un int que representa una posición en el eje y del lienzo y se usa en un triangle() que forma al tentaculo 
de Cthulhu.

- **xQuad**
Es un int que representa una posición en el eje x del lienzo y se usa en un quad() que forma al tentaculo 
de Cthulhu.

- **yQuad**
Es un int que representa una posición en el eje y del lienzo y se usa en un quad() que forma al tentaculo 
de Cthulhu.

- **validarMouse**
Es un boolean que sirve para el metodo pasarMouse().

### Metodos:
- **pintarRocas()**
Se encarga de hacer aparecer un objeto que representa unas rocas en el lienzo.

- **pintarTentaculo()**
Se encarga de hacer aparecer un objeto que representa un tentaculo de Cthulhu.

- **pasarMouse()**
Se encargan de validar para que el tentaculo pueda pintarse cuando el usuario pase el mouse sobre las rocas.

-------------------------------------------------------------------------------------------------------------------

## Clase Burbujas
Esta clase crea un objeto que representa a unas burbujas y aparecen despues de que el usuario haya dado click a una
caverna que esta en la mitad del lienzo.

### Variables:
- **x1**
Es un int que representa una posición en el eje x del lienzo y se usa en uno de los ellipse() que forma 
la burbuja.

- **y1**
Es un int que representa una posición en el eje y del lienzo y se usa en uno de los ellipse() que forma 
la burbuja.

- **x2**
Es un int que representa una posición en el eje x del lienzo y se usa en uno de los ellipse() que forma 
la burbuja.

- **x2**
Es un int que representa una posición en el eje y del lienzo y se usa en uno de los ellipse() que forma 
la burbuja.

- **tam1**
Es un int que representa el tamaño de uno de los circulos que representara una burbuja.

- **tam2**
Es un int que representa el tamaño de uno de los circulos que representara una burbuja.

- **validarMouse**
Es un boolean que sirve para validar el metodo click().

### Metodos:
- **pintarBurbuja()**
Se encarga de hacer aparecer un objeto que representa una burbuja.

- **click()**
Se encarga de validar cuando el usuario haga click y asi permita pintar las burbujas.

-------------------------------------------------------------------------------------------------------------------

## Clase Vigilant
Esta clase crea un objeto que representa al barco Vigilant el cual el usuario podra arrastrarlo hacia una posición
marcada en el lienzo.

### Variables:
- **xQuad**
Es un int que representa una posición en el eje x del lienzo y se usa en un quad() que forma al barco.

- **yQuad**
Es un int que representa una posición en el eje y del lienzo y se usa en un quad() que forma al barco.

- **xTrian**
Es un int que representa una posición en el eje x del lienzo y se usa en un triangle() que forma al barco.

- **xTrian**
Es un int que representa una posición en el eje y del lienzo y se usa en un triangle() que forma al barco.

- **xRect**
Es un int que representa una posición en el eje x del lienzo y se usa en un rect() que forma al barco.

- **yRect**
Es un int que representa una posición en el eje y del lienzo y se usa en un rect() que forma al barco.

### Metodos:
- **pintarVigilant()**
Se encarga de hacer aparecer un objeto que representa al barco Vigilant.

- **arrastrarVigilant()**
Esta función se encarga de permitir al usuario arrastrar el objeto.

- **soltarVigilant()**
Esta función se encarga de permitir al usuario soltar el objeto.

-------------------------------------------------------------------------------------------------------------------

## Clase Esferas
Esta clase crea un objeto que representa unas esferas el cual el usuario podra arrastrarlas hacia una posición en
el lienzo.

### Variables:
- **xCir**
Es un int que representa una posición en el eje x del lienzo y se usa en un ellipse() que forma una roca.

- **yCir**
Es un int que representa una posición en el eje y del lienzo y se usa en un ellipse() que forma una roca.

- **xEsf**
Es un int que representa una posición en el eje x del lienzo y se usa en un ellipse() que forma una esfera.

- **yEsf**
Es un int que representa una posición en el eje y del lienzo y se usa en un ellipse() que forma una esfera.

- **tam**
Es un int que representa el tamaño del circulo que representara una roca.

- **tamE**
Es un int que representa el tamaño del circulo que representara una esfera.

- **validarClick**
Es un boolean que se usara en el metodo clickRocas().

### Metodos:
- **pintarEsferas()**
Se encarga de hacer aparecer un objeto que representa a una esfera.

- **pintarRocas()**
Se encarga de hacer aparecer un objeto que representa a unas rocas.

- **clickRocas()**
Se encarga de validar cuando el usuario haga click sobre las rocas en el lienzo y pueda hacer aparecer las esferas.

- **arrastarEsfera()**
Permite al usuario arrastrar las esferas con el mouse.

- **soltarEsfera()**
Permite al usuario soltar las esferas en la posición que desee.

- **rotarEsfera()**
Hace que las esferas giren en torno a Cthulhu cuando son arrastradas a cierta posición.