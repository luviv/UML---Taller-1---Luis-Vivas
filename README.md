# Taller 1 DCA - Luis �ngel Vivas

## Clase Main
Es la clase encargada de llamar a todos los metodos y clases para poder ejecurtar el programa.

### Metodos:
- **settings()**
Metodo utilicado para definir los parametros de size() que define el tama�o del lienzo.

- **setup()**
La funci�n setup () se ejecuta una vez, cuando se inicia el programa. Se utiliza para definir las propiedades 
del entorno inicial.

- **draw()**
La funci�n ejecuta continuamente las l�neas de c�digo contenidas dentro de su bloque hasta que se detiene 
el programa.

- **mousePRessed()**
La funci�n se llama una vez despu�s de cada vez que se presiona un bot�n del mouse.

- **mouseDragged()**
La funci�n se llama una vez cada vez que se mueve el mouse mientras se presiona un bot�n del mouse.

- **mouseReleased()**
La funci�n se llama cada vez que se suelta un bot�n del mouse.

- **mouseClicked()**
La funci�n se llama despu�s de presionar un bot�n del mouse y luego liberarlo.

- **mouseMoved()**
Se llama a la funci�n cada vez que se mueve el mouse y no se presiona el bot�n del mouse.

- **keyPressed()**
La funci�n se llama una vez cada vez que se presiona una tecla. La tecla presionada se almacena en la 
variable clave.

-------------------------------------------------------------------------------------------------------------------

## Clase Logica
Es la clase encargada de instanciar, llamar y operar las dem�s clases en las que se crearan objetos.

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
Esta funci�n contiene al texto y lo analiza para desprender las interacciones.

- **pintar()**
Muestra todos los elementos en el lienzo.

- **arrastrar()**
Se encarga de todos los eventos del mouse que tengan que ver con la acci�n de arrastrar.

- **soltar()**
Se encarga de todos los eventos del mouse que tengan que ver con la acci�n de soltar despues de presionar click.

- **click()**
Se encarga de todos los eventos del mouse que tengan que ver con la acci�n de hacer click.

- **clickPresionado**
Se encarga de todos los eventos del mouse que tengan que ver con la acci�n de mantener presionado el click.

- **pasarMouse**
Se encarga de todos los eventos del mouse que tengan que ver con la acci�n de pasar el mouse en cierta area.

- **presionarTecla**
Se encarga de todos los eventos del teclado que tengan que ver con la acci�n de apresionar una tecla.

-------------------------------------------------------------------------------------------------------------------

## Clase Estrellas







  