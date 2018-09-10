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







  