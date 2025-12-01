<p align="center">
    <img src="./learn-gopher-nbg.png" height="300px" width="200px" alt="gopher" >
</p>

# Aprende Go (Golang)

### Consideraciones

**Sobre el contenido:**
- Todo el material está basado en los recursos oficiales de Go listados en la sección de Referencias
- El contenido se presenta resumido y simplificado para tratar de facilitar el aprendizaje
- Algunos conceptos se repiten en diferentes secciones con distintos niveles de profundidad, reflejando la naturaleza de los recursos originales
- Los recursos originales están en inglés; la traducción busca ser precisa pero puede contener interpretaciones personales

**Sobre este repositorio:**
- **NO es un curso formal**, sino una documentación personal de mi propio aprendizaje de Go
- Puede contener imprecisiones o interpretaciones personales de los conceptos
- Ante cualquier duda, consulta siempre los recursos oficiales

¡Disfruta tu aprendizaje!

---

# Índice

## Sección 1: A Tour Of Go

### Lo básico

- Paquetes
- Nombres exportados (públicos y privados)
- Funciones
  - Funciones como valores
  - Funciones closure
- Variables
- Valores cero (Zero values)
- Tipos básicos
- Conversión de tipo
- Constantes
- Constantes numéricas
- Bucles
  - Bucle for
  - Bucle while
- Condición if
- Switch
- Defer
- Punteros
- Structs
- Arreglos
- Slices
- Mapas
- Range

### Métodos e Interfaces

- Métodos
- Interfaces
- Aserción de tipos
- Switches de tipo
- Stringers
- Errores
- Lectores
- Escritores
- Imágenes

### Genéricos

- Tipos de parámetro
- Tipos genéricos

### Concurrencia

- Rutinas go
- Canales
- Canales con buffer
- Range y Close
- Select

## Sección 2: How to Write Go Code

- Organización del código
- Tu primer programa
  - Importar paquetes del mismo módulo
  - Importar paquetes de módulos externos
- Pruebas

## Sección 3: The Go Programming Language Specification

### Introducción

### Representación del código fuente

### Elementos léxicos

- Comentarios
- Tokens
- Punto y coma
- Identificadores
- Palabras reservadas
- Operadores y puntuación
- Enteros literales
- Puntos-flotantes literales
- Imaginarios literales
- Rune literales
- String literales

### Constantes

### Variables

### Tipos

- Tipo booleano
- Tipo numérico
- Tipo string
- Tipo arreglo
- Tipo slice
- Tipo struct
- Tipo puntero
- Tipo función
- Tipos interfaz
  - Interfaces básicas
  - Interfaces embebidas
  - Interfaces genéricas
- Tipo mapa
- Tipo canal

### Propiedades de tipos y valores

- Representación de valores
- Tipos subyacentes
- Tipos base
- Identidad del tipo
- Asignabilidad
- Representabilidad
- Conjunto de métodos

### Bloques

### Declaraciones y alcance

- Alcance de etiquetas
- Identificador en blanco
- Identificadores predeclarados
- Identificadores exportados
- Unicidad de los identificadores
- Declaración de constantes
- Iota
- Declaraciones de tipo
  - Declaración de alias
  - Definición de tipos
- Declaración de tipos de parámetro
  - Restricciones de tipo
  - Cumplimiento de las restricciones de tipo
- Declaración de variables
- Declaración corta de variables
- Declaración de funciones
- Declaración de métodos

### Expresiones
- Operandos
- Identificadores calificados
- Literales compuestos
- Funciones literales
- Expresiones primarias
- Selectores
- Expresiones de métodos
- Valores de métodos
- Expresiones de índice
- Expresiones de slice
  - Expresiones de slice simples
  - Expresiones de slice completas
- Aserción de tipos
- Expresión de llamadas
- Pasando argumentos a parámetros "..."
- Instanciaciones
- Inferencia de tipos
  - Unificación de tipos
- Operadores
  - Precedencia de operadores
- Operadores aritméticos
  - Operadores de enteros
  - Desbordamiento de enteros
  - Operadores de punto-flotante
  - Concatenación de strings
- Operadores de comparación
- Operadores lógicos
- Operadores de dirección
- Operador de recepción
- Conversiones
  - Conversiones entre tipos numéricos
  - Conversiones de y hacia tipos string
  - Conversiones de slice a arreglo
- Expresiones constantes
- Orden de evaluación

### Sentencias

- Sentencias de terminación
- Sentencias vacías
- Sentencias etiquetadas
- Sentencias expresivas
- Sentencias de envío
- Sentencias de incremento/decremento
- Sentencias de asignación
- Sentencias if
- Sentencias switch
  - Switch de expresión
  - Switch de tipo
- Sentencias for
  - Sentencias for con una única condición
  - Sentencias for completas
  - Sentencias for usando range
- Sentencias go
- Sentencias select
- Sentencias return
- Sentencias break
- Sentencias continue
- Sentencias goto
- Sentencias fallthrough
- Sentencias defer

### Funciones integradas

- Añadir a y copiar slices
- Clear
- Close
- Manipulación de números complejos
- Eliminación de elementos de un mapa
- Longitud y capacidad
- Crear mapas, slices y canales
- Mínimo y máximo
- Asignación de memoria
- Gestionar pánicos
- Arranque

### Paquetes

- Optimización de archivos fuente
- Package
- Declaraciones de importación

### Inicialización y ejecución de un programa

- El valor cero
- Inicialización de un paquete
- Inicialización de un programa
- Ejecución de un programa

### Errores

### Pánicos en tiempo de ejecución

### Consideraciones de sistema

- Paquete unsafe
- Garantías de tamaño y alineación

## Sección 4: Effective Go

### Formateo

### Comentarios

### Nombres

- Nombres de paquetes
- Getters y Setters
- Nombres de interfaces
- MixedCaps

### Punto y coma

### Estructuras de control

- If
- Re-declaración y re-asignación
- For
- Switch
- Switch de tipo

### Funciones

- Múltiples valores de retorno
- Parámetros nombrados de resultado 
- Defer

### Datos

- Asignación con new
- Constructores y literales compuestas
- Asignación con make
- Arreglos
- Slices
- Slices de dos dimensiones
- Mapas
- Imprimir
- Append

### Inicialización

- Constantes
- Variables
- Función init

### Métodos

- Punteros vs. Valores

### Interfaces y otros tipos

- Interfaces
- Conversiones
- Conversión de interfaces y aserción de tipos
- Generalidad
- Interfaces y métodos

### El identificador en blanco

- El identificador en blanco en asignaciones múltiples
- Importaciones y variables sin usar
- Importar para efectos secundarios
- Chequeo de interfaces

## Referencias

---

# Sección 1: A Tour Of Go

## Lo básico

### Paquetes

Cualquier programa de Go se compone de **paquetes**, los cuales, son básicamente directorios que contienen archivos de código con algún tipo de relación o parecido. Además, el punto de entrada de cualquier programa **ejecutable** debe ser el paquete `main`.

Por convención, el nombre de cualquier paquete es el mismo que el último elemento de la ruta de importación.
- Ejemplo:
    - Ruta de importación: `math/rand`
    - Nombre del paquete: `package rand`

### Nombres exportados (públicos y privados)

En Go, un nombre declarado dentro un paquete, ya sea de una función, constante, etc., solo va a ser exportado si ese nombre inicia con una letra mayúscula. Básicamente, que un nombre inicie con mayúscula lo hace público. Por lo tanto, al importar un paquete, solo se pueden usar los nombres exportados.
- Ejemplo:
    - `Pi` es un nombre exportado (público)
    - `pi` no es un nombre exportado (privado)

### Funciones

Las funciones pueden tomar cero o más argumentos, y su funcionamiento es muy parecido al de cualquier otro lenguaje de programación. Sin embargo, es importante tener en cuenta que la sintáxis es diferente, pues en Go, primero se pone el nombre del argumento y luego el tipo de dato, contrario a lo usual.

De acuerdo al artículo del blog de Go [Go's Declaration Syntax](https://go.dev/blog/declaration-syntax), estas son las razones por las que su sintáxis es diferente a la de otros lenguajes populares, como los lenguajes de la familia C:
- La sintáxis de los lenguajes de la familia C para la declaración de identificadores, como variables o funciones, **envuelve** el nombre de los items, pues el especificador de tipo de dato está a la izquierda del nombre y otras características o valores están a su derecha. Esto, si bien es una forma inusual e inteligente, para algunos casos, esta forma hace que la legibilidad del código se dificulte bastante
- La sintáxis de declaración en Go, toma la idea base donde los nombres están primero (izquierda) y sus especificadores de tipo de dato después (derecha). Por lo tanto, con esta idea base, la legibilidad **izquierda-a-derecha** se vuelve muy sencilla y se da naturalmente, en comparación con C, donde se envuelven los nombres y se vuelve difícil de leer
- Por otro lado, los punteros son un punto de excepción, pues no puedieron hacer esa reversión de sintáxis, por lo que estos funcionan como lo hacen en C: con la notación `*` y siendo usados antes del nombre del puntero
    - Ejemplo:
        ```Go
        var p *int
        x = *p
        ```

También, las funciones pueden retornar múltiples valores, siempre y cuando se declaren dentro de paréntesis `()`. Estos valores pueden obtener su significado de acuerdo a su posición o mediante un nombre. Cuando los valores de retorno son nombrados, son tratados como si fueran variables definidas al inicio de la función.
- Ejemplo:
    ```Go
    func funcionRetorno(p1 string, p2 int) (r1 string, r2 int) {
        r1 := p1 + " modificado"
        r2 := p2 + 5
        return // r1 y r2 se devuelven automáticamente porque son valores de retorno nombrados
    }
    ```

#### Funciones como valores

Las funciones también son valores, como cualquier otro valor (int, string, array, etc), por lo que pueden ser asignadas a variables como si fuera un valor normal. Incluso, también pueden ser usadas como argumentos de otras funciones o como valores de retorno de funciones.

#### Funciones closure

Las funciones además, pueden ser **closures** de otras funciones, es decir, que pueden actuar como funciones anónimas que utilizan variables fuera de su alcance (correspondientes a su función padre) y que son regresadas por su misma función padre. Esto provoca que el estado de las variables utilizadas dentro del **closure** que pertenecen a la función padre mantengan su estado hasta que esa función **closure** ya no se use más.

### Variables

Para declarar las variables se utiliza la palabra reservada `var`, la cual, declara puede declarar una o más variables variables, y se debe usa la misma sintáxis de **izquierda-a-derecha**, es decir, poner el tipo de variable al final, y si son múltiples variables del mismo tipo, solo se debe poner al final una vez.

La declaración con `var` puede ser usada en varios niveles (scope), ya sea a nivel de paquete o de función, y puede incluir inicializadores (valores iniciales), uno por variable. Cuando los inicializadores se presentan en la declaración de variables, el especificador del tipo de la variable puede ser omitido, ya que tomará el valor de ese inicializador.

- Ejemplo:
    ```Go
    // Declaración de variables sin inicializador
    var miVariable1 string
    var miVariable2 int
    ```
    ```Go
    // Declaración de variables con inicializador
    var miVariable1 string = "mi variable"
    var miVariable2 int = 10
    ```
    ```Go
    // Declaración de múltiples variables del mismo tipo con inicializadores
    var miVar1, miVar2, miVar3 int = 10, 11, 12
    ```

Además, se puede usar el operador `:=` dentro del bloque (scope) de una función para reemplazar la declaración de `var` y utilizar de forma implícita el tipo del valor asignado para simplificar la declaración e inicialización de variables. Sin embargo, es importante considerar que fuera del bloque (scope) de funciones, es decir, a nivel de paquete todas las declaraciones deben iniciar con alguna palabra reservada, por lo que el uso de este operador a nivel de paquete no es posible.
- Ejemplo:
    ```Go
    func bloqueFuncion() {
        miVariable1 := "variable tipo string"
    }
    ```

### Valores cero (Zero values)

Las variables que son declaradas sin un inicializador (valor inicial) explícito se les asigna un **valor cero (zero value)**, es decir, una valor por defecto que depende del tipo de la variable.
- Ejemplo:
    - Variables numéricas: `0`
    - Variables booleanas: `false`
    - Variables string: `""`

### Tipos básicos

Go tiene los siguientes tipos de datos, representados en ocho diferentes categorías:
- Booleano: `bool`
- String: `string`
- Numérico: `int`, `int8`, `int16`, `int32`, `int64`
- Numérico sin signo: `uint`, `uint8`, `uint16`, `uint32`, `uint64`, `uintptr`
- Byte: `byte` == `uint8`
- Rune: `rune` == `int32`
- Flotante: `float32`, `float64`
- Complejo: `complex64`, `complex128`

Generalmente, los tipos que no tienen un tamaño especificado, como `int`, `unit` o `uintptr` dependen del Sistema Operativo, ya que su tamaño puede ser de 32-bits o 64-bits. Por lo tanto, Go recomienda usar estos tipos sin tamaño específico cuando se requiera utilizar un valor numérico, a menos que haya razones específicas para usar otro tipo.

### Conversión de tipo

Para convertir un tipo a otro tipo se utiliza la expresión `T(v)`, donde `v` es el valor a convertir y `T` es el tipo al que se va a convertir.
- Ejemplo:
    ```Go
    var entero int = 42
    var flotante float64 = float64(entero)
    var nosigno uint = uint(flotante)
    ```

A diferencia de otros lenguajes, como C, la asignación de valores de diferentes tipos en Go requiere explícitamente la conversión de los tipos. Por lo tanto, es evidente que el casteo (conversión) no se hace automáticamente.

### Constantes

Las constantes son declaradas de forma similar a las variables, con la diferencia de que se debe utilizar la palabra reservada `const`. Además, estas debido a que siempre deben usar la palabra reservada `const`, no pueden usar el operador de asignación corta `:=`.
- Ejemplo:
    ```Go
    const CONSTANTE = "MI CONSTANTE"
    ```

### Constantes numéricas

Las constantes numéricas funcionan como los constantes normales, pues tienen que ser declaradas usando la palabra reservada `const`. Sin embargo, estas constantes númericas son valores de alta precisión (high-precison values). Aquellas constantes en las que no se especifique su tipo, tomarán su tipo de valor dependiendo del contexto en el que sean usadas. Por ejemplo, si se declara una constante numérica sin su tipo y es utilizada por una función que recibe un `int` y otra que recibe un `float64`, actuará de forma correpondiente a dichas funciones.

### Bucles

#### Bucle for

Go solo tiene una palabra reservada para un único tipo de bucle: `for`. Su uso no requiere paréntesis y sus tres componentes, si están presentes, deben ser separados por punto y coma `;`. Las tres partes del bucle **for** son:
* ***Sentencia inicial***: Esta es ejecutada antes de realizar la primera iteración del bucle. Ejemplo: `i := 0`
* ***Expresión de condición***: Esta es evaluada antes de cada iteración. Ejemplo: `i < 10`.
* ***Sentencia posterior***: Esta es ejecutada al final de cada iteración. Ejemplo: `i++`.
    ```Go
    for i := 0; i < 10; i++ {
        // Código a ejecutar en cada iteración
    }
    ```

En este tipo de bucles, tanto la **sentencia inicial** como la **sentencia posterior** son opcionales, por lo que pueden ser omitidas asegurando que la **expresión de condición** pueda terminar el bucle.

#### Bucle while

En Go no existe una palabra reservada para el bucle **while**, pues para simular su funcionamiento se usa `for`, ya que este bucle permite declarar únicamente la expresión de condición que hace que el bucle continúe. Sin embargo, es importante tener en cuanta que para cualquier tipo de bucle que utilice la palabra reservada `for`, si se omiten todos sus componentes se convierte en un bucle infinito.

### Condición if

La estructura de este tipo de condición es muy parecida a la estructura del bucle `for`, pues las condiciones `if` no necesitan estar entre paréntesis, pero sí es obligatorio que su cuerpo esté entre llaves `{}`. Además, pueden iniciar con una **sentencia inicial** que se ejecuta antes de evaluar la condición, pero es importante tener en cuenta que las variables declaradas inicialmente en la condición solamente están en al alcance del bloque **if** donde fueron declaradas (incluyendo `else`).
- Ejemplo:
    ```Go
    if resultado := 10; resultado < 20 {
        // Código a ejecutar si la condición se cumple
    }
    ```

### Switch

Esta declaración funciona como en la mayoría de lenguajes y se usa la palabra reservada `switch`. Sin embargo, Go únicamente ejecuta el `case` donde la condición es cumplida y no continua con la ejecución de los siguientes casos, por lo que el uso de `break` en cada caso es automáticamente hecho por Go.

Go evalúa las condiciones de arriba hacia abajo, y se detiene en la condición que se cumpla, y no continuará ejecutando las condiciones restantes, como lo hacen otros lenguajes como C. También, es posible usar un `switch` sin una condición, y eso será evaluado como un `true`.
- Ejemplo:
    ```Go
    opcion := "APAGADO"
    switch opcion {
    case "ENCENDIDO":
        // Código a ejecutar si el caso se cumple
    case "APAGADO":
        // Código a ejecutar si el caso se cumple
    default:
        // Código a ejecutar si ninguno de los casos se cumple
    }
    ```

### Defer

La función `defer` hace que la ejecución de la función que se indique sea realizada inmediatamente antes de que la función en la que se usa **defer** finalice o retorne su resultado. Además, este tipo de funciones utiliza un stack especial y utiliza el orden `LIFO` (Last In - First Out), lo que es crucial para entender el funcionamiento y orden de ejecución de las funciones **defer**.

### Punteros

Los punteros almacenan la dirección de memoria de un objeto. Es decir, que un puntero apunta a la dirección de memoria donde es almacenado un objeto, y es importante entender que no apunta directamente al valor, sino a la dirección de memoria. Cabe resaltar que a diferencia de C, Go no tiene aritmética de punteros.

Para trabajar con punteros hay dos operadores clave:
- `*`: Este operador indica que un objeto es un puntero a cierto tipo. Por ejemplo:
    ```Go
    var p *int // Donde p apunta a una dirección de memoria que almacena un valor de tipo int
    ```
- `&`: Este operador obtiene la dirección de memoria de un objeto. Por ejemplo:
    ```Go
    var i int = 42
    p = &i // Donde &i obtiene la dirección de memoria del objeto i
    ```
- Al trabajar con punteros, se pueden trabajar con dos valores diferentes, de distinta forma
    - Si se quiere usar la dirección a la que apunta, se usa el nombre del puntero (`p`)
    - Si se quiere usar el valor de la dirección de memoria a la que apunta, se usa el operador de desreferenciación y el nombre del puntero (`*p`)

### Structs

Una estructura es una colección de **miembros (fields)**, y para acceder a los miembros de una estructura de usa la notación de punto `.` y el nombre exacto del miembro.
- Ejemplo:
    ```Go
    type Estructura1 struct {
        Campo1 int
        Campo2 string
    }
    var estructura Estructura1 = Estructura1{ 1, "nombre" }
    ```

Los punteros que almacenan la dirección de memoria de una estructura se comportan de manera un poco diferente. Pues, normalmente, para acceder a los miembros de una estructura mediante un puntero se utilizaría la expresión `(*p).X`, sin embargo, Go permite una expresión más sencilla `p.X`. Esto es posible ya que una estructura es la dirección de memoria base del bloque donde se almacenan todos sus miembros, y para acceder a ellos se utilizan desplazamientos (offsets) basados en el tipo de dato del miembro y del padding agregado por el compilador.
- Ejemplo:
    ```Go
    (*p).X = 3 // Forma real para acceder a un miembro usando un puntero a una estructura
    p.Y = 4    // Forma simplificada para acceder a un miembro usando un puntero a una estructura
    ```

Al crear una variable de tipo estructura, se pueden dar tres casos:
- Se pueden especificar los valores de uno o más miembros de una estructura de forma posicional, es decir, que los valores serán asignados dependiendo del orden de declaración de los miembros. Ejemplo:
    ```Go
    v1 := Estructura1{ 5, "campo" } // Campo1 = 5, y Campo2 = "campo"
    ```
- Se pueden especificar los valores de uno o más miembros de una estructura usando sus nombres, lo que resulta más claro y en algunos casos, más conveniente. Ejemplo:
    ```Go
    v2 := Estructura1{ Campo1: 7, Campo2: "campo" }
    ```
- Si no se especifican los valores de uno o más miembros de una estructura, a dichos miembros se les asignará su **valor cero (zero value)**. Ejemplo:
    ```Go
    v3 := Estructura1{} // Campo1 = 0, y Campo2 = ""
    ```
- **Nota**: No es posible combinar los dos primeros casos para asignar valores, se debe usar únicamente una forma de asignar valores, ya sea usando su posición o usando su nombre

### Arreglos

Los arreglos en Go funcionan de forma completamente diferente a los arreglos en C. Pues en C, un array siempre se utiliza por referencia, es decir, por su dirección de memoria; mientras que en Go, un array simpre se utiliza por valor, por lo que siempre se apunta a todos los valores del array en lugar de su dirección base.

Entonces, para declarar un array se utiliza la expresión `[n]T`, donde `n` es la cantidad de elementos del array, y `T` es el tipo de valor de los elementos. El tamaño del arreglo es parte de su tipo, por lo que son de tamaño fijo.
- Ejemplo:
    ```Go
    var arreglo1 [3]int // Arreglo de dos tres elementos de tipo entero
    arreglo1[0], arreglo1[1], arreglo1[2] = 3, 4, 5
    ```

### Slices

Un slice es como un arreglo pero de tamaño dinámico y es una forma flexible de acceder a los elementos del arreglo subyacente que usa el slice. Un slice es formado al especificar dos índices: **límite inferior (low bound)** y **límite superior(high bound)** separados por dos puntos `:`. Por defecto, el valor cero de **límite inferior** es `0`, y el del **límite superior** es la longitud del arreglo subyacente del slice.
- Ejemplo:
    ```Go
    arregloSubyacente := [6]int{1, 2, 3, 4, 5, 6}
    var slice1 []int = arregloSubyacente[1:4] // {2, 3, 4}
    // Slice de 3 elementos, donde se incluye el límite inferior pero no el límite superior
    ```

A diferencia de un arreglo, un slice no almacena realmente los valores, sino que describe una sección de un arreglo existente o completo, es decir, que trabaja con la referencia (dirección de memoria) de un arreglo. Por lo tanto, como un slice trabaja con una referencia, al modificar el slice, el arreglo y otros slices dependientes cambian de igual forma.

Cualquier slice tiene dos características fundamentales:
* **Longitud**: La longitud es el número de elementos que contiene el slice. Se usa la función `len()` para obtener la longitud
* **Capacidad**: La capacidad es el número de elementos que contiene el arreglo subyacente contando desde el primer elemento del que parte el slice. Se usa la función `cap()` para obtener la capacidad

El valor cero de un slice es `nil`, y un slice vacío tiene una longitud y capacidad de 0, ya que no existe un array del cual partir.

Otra forma de crear slices es con la función integrada `make()`, pues esta se encarga de alojar un arreglo del tamaño especificado, llenarlo con valores cero y devolver un slice que usa la referencia del arreglo creado.
- Ejemplo:
    ```Go
    slice2 := make([]int, 0, 5) // Crea un slice de elementos int, con longitud de 0 y capacidad de 5
    ```

Go integra también la función `append()` para agregar nuevos elementos a un slice. Esta función recibe el slice al cual se le van a agregar los elementos, y recibe los elementos a agregar. El resultado de esta función es un slice que contiene los elementos originales más los nuevos elementos agregados; si la capacidad del arreglo subyacente no puede soportar los nuevos elementos, se crea uno nuevo para poder almacenar todos los elementos y se utiliza ese nuevo arreglo.
- Ejemplo:
    ```Go
    var slice3 []int
    slice3 = append(slice3, 0, 1)
    slice3 = append(slice3, 2, 3, 4)
    ```

### Mapas
Un `map` es básicamente un arreglo de valores que son accedidos mediante llaves en lugar de índicies, por lo que toman la forma de **llave-valor**.

El valor cero de un mapa es `nil`, y cuando un mapa que tiene este valor, no tiene nada de contenido y da error si se trata de agregar contenido. Sin embargo, se puede utilizar la función `make` para crear un mapa vacío usable, pues esta función devuelve un mapa de cierto tipo inicializado y listo para ser usado.
- Ejemplo:
    ```Go
    mapa := make(map[string]int) // Mapa inicializado sin contenido, con llaves de tipo string y elementos de tipo int
    ```

Se pueden realizar varias operaciones con los mapas, como:
* Insertar o Actualizar un elemento del mapa:
    ```Go
    mapa["Llave"] = 42
    // Si la llave "Answer" existe, actualiza el valor
    // Si la llave "Answer" no existe, crea la llave y asigna el valor
    ```
* Obtener un elemento del mapa:
    ```Go
    valor = mapa["Llave"]
    // Regresa el valor correspondiente a la llave "Answer"
    ```
* Eliminar un elemento del mapa:
    ```Go
    delete(mapa, "Llave")
    ```
* Verificar que una llave exista en el mapa:
    ```Go
    value, ok := m["Llave"]
    // Si existe, regresa el valor y la segunda variable es true
    // Si no existe, regresa el zero value y la segunda variable es false
    ```

### Range

Utilizar la palabra reservada `range` es una forma corta de recorrer los elementos de un arreglo, slice o mapa, incluso de recorrer un rango numérico. Cuando se utiliza para recorrer algún objeto iterable, se obtienen dos valores: el index o llave del elemento, y una copia del propio elemento.

Alguno de los dos valores que se obtienen de usar `range` puede ser ignorado usando el identificador en blanco `_` o simplemente omitiendo la variable donde se almacenaría dicho elemento (siempre y cuando no sea el primer valor retornado).
- Ejemplo:
    ```Go
    mapa := make(map[string]string)
    for index, valor := range mapa {
        // Usar el index y valor del mapa
    }
    ```

## Métodos e Interfaces

### Métodos

Go no tiene Programación Orientada a Objetos (POO) y por lo tanto, no tiene clases ni objetos. Sin embargo, es posible relacionar métodos a los tipos, pues un método es básicamente una función pero con un **argumento receiver** especial que aparece después de la palabra reservada `func` pero antes del nombre del método. Dicho **argumento receiver** asocia el método con el tipo de ese argumento, es decir, especifica qué tipo posee el método declarado.
- Ejemplo:
    ```Go
    // Tipo: Estructura1
    type Estructura1 struct {
        Campo1, Campo2 float64
    }

    // Método asociado y usable únicamente desde un tipo Estructura1
    func (e1 Estructura1) Suma() float64 {
        return e1.Campo1 + e1.Campo2
    }
    ```

Los métodos pueden ser declarados con cualquier tipo, siempre y cuando dicho tipo se encuentre definido en el mismo paquete donde se declara el método; y que no sea un tipo predefinido por el lenguaje, como **int** o **string**.

Entonces, básicamente un método es una función que recibe un objeto de cierto tipo y dicho método es asociado al tipo del objeto recibido, no a la propia instancia del objeto. Existen dos formas por las que un método puede recibir el objeto de cierto tipo:
- **Value receiver**: Cuando se recibe un objeto por valor, se está recibiendo una copia del objeto, por lo tanto, nunca se puede trabajar ni modificar el objeto real
- **Pointer receiver**: Cuando se recibe un objeto por referencia o puntero, se está recibiendo la dirección de memoria del objeto real, por lo tanto, se trabaja con el objeto real y cualquier modificación será visible en otras partes que usen el mismo objeto
* **Nota:** Un método debe usar o value receivers o pointer receivers, pero no se deben combinar.

### Interfaces

Una interfaz es un objeto de tipo `interface` que define un conjunto de métodos a implementar. Es decir, que una interfaz es un contrato de métodos, y cualquier tipo que implemente los métodos declarados en la interfaz puede usar dicha interfaz.

Es importante mencionar que toda interfaz almacena información sobre el objeto que la usa en forma de tupla, pues almacena el valor de dicho objeto y el tipo del objeto para saber a qué método debe llamar: `(valor, tipo)`.

Las interfaces son implementadas cuando un tipo implementa los métodos de dicha interfaz, por lo que no se necesitan palabras clave o declaraciones explícitas. Además, cuando se llama a un método implementado por la interfaz, se ejecuta el método que tiene nombre específico y el tipo específico, por lo que una interfaz guarda la información del tipo que implementan sus métodos.

Un objeto de tipo interfaz está vacío `nil` si no tiene nada de información en su tupla `(valor, tipo)`, y llamar a algún método de esta interfaz causa un pánico en el programa, ya qu Go no sabe qué método invocar.

Existen también las interfaces vacías que no implementan ningún método declaradas con el tipo `any`, son conocidas como **interfaces vacías** y pueden guardar valores de cualquier tipo.

### Aserción de tipos

Las aserciones de tipo básicamente se usan para verificar que un objeto sea de un tipo específico, y proveen acceso al tipo de dato del objeto y a su valor. Cabe mencionar que estas operaciones son posibles únicamente en objetos de tipo `interface`, pues son los tipos que no tienen tipos específicos en todo momento.
- Ejemplo:
    ```Go
    valor := obj.(TIPO) // Donde obj es el objeto de tipo interface y TIPO es el tipo que se quiere asegurar (int, string, etc.)
    ```

En el ejemplo anterior, la aserción se asegura de que el tipo del valor de un objeto de una interfaz es de cierto tipo, y asigna el valor a la variable si es que la aserción es verdadera. En caso contrario de que el objeto no sea del tipo especificado se produce un error.

Sin embargo, existe otra forma de usar las aserciones de tipo para ver si el objeto de una interfaz es de un tipo específico:
```Go
valor, ok := obj.(TIPO)
```

En este caso, la aserción regresa el valor del objeto del tipo especificado a la variable y también regresa `true` si es que es verdad; pero si el objeto de la interfaz no es del tipo especificado (T), regresa el valor cero del tipo y `false` (ok), pero no se produce ningún error.

### Switches de tipo

Usar `type` dentro de los switches es un constructo que permite realizar varias **aserciones de tipo** con varios tipos. En estos casos, el funcionamiento es exactamente el mismo que cualquier otro switch, con la diferencia de que los casos evalúan diferentes tipos en lugar de valores, y se usa la palabra reservada `type` dentro de la aserción.
- Ejemplo:
    ```Go
    func switchTipo(obj any) {
        switch valor := obj.(type) {
        // La variable valor toma el valor del objeto de la interfaz y puede ser usada dentro de cualquier caso
        case int:
            // El objeto de la interfaz es de tipo int.
        case string:
            // El objeto de la interfaz es de tipo sring.
        default:
            // El objeto de la interfaz es de otro tipo.
        }
    }
    ```

### Stringers

Dentro del paquete `fmt` se encuentra definida la interfaz `Stringer`. Esta interfaz implementa el método `String()`, y cualquier objeto que la implemente puede describirse a sí mismo como un string. El paquete `fmt` y muchos otros buscan esta interfaz en los objetos cuando se imprime dicho objeto, por lo que no es necesario llamar al método explícitamente.
```Go
type Stringer interface {
    String() string
}
```

### Errores

Los programas en Go expresan estados de error con valores de tipo `error`. Este tipo es una interfaz ya integrada en el lenguaje e implementa el método `Error()`, similar al método implementado por la interfaz **Stringer**, el paquete `fmt` y otros buscan este método al momento de imprimir objetos de tipo error.
```Go
type error interface {
    Error() string
}
```

Generalmente, las funciones regresan un tipo `error` como último o único valor de retorno, por lo que el código siempre debería manejar y considerar los errores al verificar dicho valor es igual a `nil` o no.
- Ejemplo:
    ```Go
    num, err := strconv.Atoi("42")
    if err != nil {
        // La función devolvió un error (error != nil)
    }
    // La función no devolvió un error (error == nil)
    ```

### Lectores

El paquete `io` especifica la interfaz `io.Reader`, que representa la lectura de un flujo de datos hasta su fin. La librería estándar de Go tiene muchas implementaciones de esta interfaz, como archivos, conexiones de red, compresores, cifrados, etc. Lo que hace el método `Read` es llenar un slice de bytes con información y regresar el número de bytes con los que fue llenado el slice, también, regresa un valor de tipo `error`. Cuando el flujo de datos termina, simplemente regresa un `error` de tipo `io.EOF`.
```Go
func (t T) Read(b []byte) (n int, err error)
```

### Escritores

El paquete `io` también especifica la interfaz `io.Writer`, que representa la escritura de un flujo de datos hasta su fin en un cierto destino.

Lo que hace el método `Write` es escribir los datos desde un slice de bytes hacia un cierto destino, también regresa el número de bytes escritos y un valor de tipo `error`, que puede contener errores al momento de hacer la escritura.
```Go
func (t T) Write(b []byte) (n int, err error)
```

### Imágenes

El paquete `image` define la interfaz `Image`, que sirve para representar algunas de las características de las imágenes.
```Go
type Image interface {
    ColorModel() color.Model
    Bounds() Rectangle
    At(x, y int) color.Color
}
```

## Genéricos

### Tipos de parámetro

Las funciones en Go pueden usar **tipos de parámetro** para trabajar con tipos genéricos que permiten múltiples tipos. Los **tipos de parámetro** se definen entre `[]` después del nombre de la función y antes de sus argumentos.
- Ejemplo:
    ```Go
    // Parámetro de tipo T que implemente la interfaz comparable
    func Index[T comparable](s []T, x T) int {
        for i, v := range s {
            if v == x {
                return i
            }
        }
        return -1
    }
    ```

Los **tipos de parámetro** pueden tener restricciones que limitan qué tipos pueden usar:
* `comparable`: Permite usar `==` y `!=`
* `any`: Acepta cualquier tipo (sin restricciones)
* **Constraints personalizadas:** Interfaces que definen métodos requeridos

### Tipos genéricos

También se pueden crear tipos genéricos (structs, interfaces, etc.) que funcionen con múltiples tipos.
- Ejemplo:
    ```Go
    type Generico[T any] struct {
        items []T
    }

    genericoEnteros := Generico[int]{ items: []int{ 1, 2, 3 } }
    genericoStrings := Generico[string]{ items: []string{ "a", "b", "c" } }
    ```

## Concurrencia

### Rutinas go
Una **rutina go (goroutine)** es un hilo ligero manejado por Go en tiempo de ejecución. Básicamente, es una función que se ejecuta concurrentemente (al mismo tiempo) en el programa y se crean usando la palabra reservada `go`.

La evaluación de los argumentos de dicha función es realizada en la **rutina go actual** en donde se crea la **nueva rutina go** a ser ejecutada, por lo que la ejecución de dicha función ocurre en esa **nueva rutina go** y el momento en que se ejecutan es completamente decidido por el **planificador (scheduler)** de Go. No son realmente ejecutadas inmediatemente después de crearlas ni después de evaluarlas, sino cuando el **planificador** así lo decide.
```Go
func rutinaActual() {
    go rutinaNueva() {
        // Código a ejecutar concurrentemente
    }
}
```

Todas las **rutinas go** son almacenadas en el mismo espacio de memoria (heap), por lo que comparten dicho espacio y el acceso a esta memoria compartida debe ser sincronizado. Sin embargo, cada rutina cuenta con su propio espacio de memoria (stack) para almacenar los objetos utilizados en la función que ejecuta.

Un punto que pasa por desapercibido, es que Go, automáticamente mueve las variables del programa que se encuentran en el **stack** al **heap** cuando detecta que esas variables son utilizadas por al menos una **rutina go**, a esto se le llama **escape analysis**, y provoca un uso adicional de recursos (overhead).

- Ejemplos:
    ```Go
    x := 5
    // Los argumentos se evalúan antes de crear la rutina go
    go func(val int) {
        fmt.Printf("Valor en goroutine: %d\n", val)
    }(x) // x se evalúa aquí con su valor actual 5
    x = 10 // Cambiar x no afectará en la goroutine, ya que se recibe una copia en la función de la rutina go
    ```

    ```Go
    mensaje := "Hola mundo"
    // Se mueve la variable mensaje del stack al heap ya que la rutina go la usa
    go func() {
        fmt.Println(mensaje) // Accede a la variable compartida
    }()
    ```

    ```Go
    func problemaBucle() {
        // Todas las goroutines ven el mismo valor de i, pues acceden al valor compartido en el heap
        for i := 0; i < 3; i++ {
            go func() {
                fmt.Printf("Goroutine ve i = %d\n", i)
            }()
        }
        // Resultado probable: "3 3 3" (todas ven el valor final de i)
    }

    func solucionBucle() {
        // Pasar i como argumento para capturar su valor
        for i := 0; i < 3; i++ {
            go func(val int) {
                fmt.Printf("Goroutine ve val = %d\n", val)
            }(i) // i se evalúa aquí, capturando su valor actual
        }
        // Resultado probable: "0 1 2" (en cualquier orden)
    }
    ```

### Canales

Los canales son un tipo de conducto por los que se pueden enviar y recibir valores, mediante el uso del operador de canal `<-` y son especialmente usados para la comunicación entre rutinas go. La información fluye en la dirección que apunte el operador de canal, y parecido a los mapas y slices, los canales deben ser creados antes de ser usados con la función `make()`.
- Ejemplo:
    ```Go
    canal := make(chan int) // Crear el canal donde se enviarán valores de tipo int
    go func(c *chan) {
        valor := <- c // Se recibe el valor que sea envíado por en canal
    }(canal)
    canal <- 5  // Enviar 5 al canal
    ```

Por defecto, un **canal sin buffer** bloquea todo el envío y recepción de información hasta que ambas partes del canal se encuentren listas y puedan ser completadas, lo  que permite que las goroutines se sincronicen implícitamente. Sin embargo, si el otro lado del canal nunca está listo o nunca se utiliza el canal ya sea para enviar o recibir, se produce un **deadlock**, donde todas las rutinas go se quedan esperando el resultado de un canal y cualquier ejecución se detiene debido a esa espera.

Es imporante reconocer que un canal, con la creación por defecto (sin buffer), no puede realmente almacenar ningún elemento, sino que asigna o envía el valor del canal directamente a donde se esté requiriendo dicho valor, permitiendo una sincronización implícita entre rutinas go.

### Canales con buffer

A los canales se les puede asignar un **buffer**, por lo que pueden ser capaces de realmente almacenar cierta cantidad de elementos. Como segundo elemento en la función `make` se puede especificar el tamaño del canal al crearlo.
- Ejemplo:
    ```Go
    canal := make(chan int, 100)  // Canal con un buffer máximo 100 elementos
    ```

Una rutina go que usa un **canal con buffer** se bloquea en dos casos:
- Al querer leer un valor del canal abierto pero no hay nada en el canal
- Al querer agregar un valor al canal cuando ya está completamente lleno

Los canales sin buffer son creados cuando no se proporciona el segundo argumento en la función `make()` o dicho argumento es 0.
- Ejemplo:
    ```Go
    canal1 := make(chan int)     // Genera un canal sin buffer
    canal2 := make(chan int, 0)  // Genera un canal sin buffer
    ```

### Range y Close

Naturalmente, un canal tiene un **transmisor** y un **receptor**. Por lo tanto, el **transmisor** puede usar la función `close` en el canal para indicar que ya no se van a enviar más valores por ese canal. Es decir, que sirve para cerrar un canal, lo que implica que no se puede mandar o almacenar más valores en dicho canal. Sin embargo, sí es posible seguir leyendo los valores del canal siempre y cuando siga habiendo valores.

Por otro lado, el **receptor** puede comprobar si un canal ya no contiene elementos y ha sido cerrado al recibir un segundo valor de retorno al asignar un valor del canal. Los canales nunca son cerrados automáticamente, pero es importante saber en qué casos se necesita especificar que el canal ya no va a enviar elementos y se va a cerrar.
- Ejemplo:
    ```Go
    valor, abierto := <-ch
    // Si abierto es true, todavía hay valores en el canal
    // Si abierto es false, ya no hay valores en el canal
    ```

Además, el uso de `range` en un bucle usando un canal, hace que se reciban los elementos de dicho canal repetidamente hasta que el canal es cerrado, por lo que no hace falta verificar manualmente si el canal ya ha sido cerrado o no.
- Ejemplo:
    ```Go
    for valor := range ch {
        // Trabajar con cada elemento del canal hasta que se cierre
    }
    ```

Pero, hay que tener cuidado con la lectura de un canal dentro de un bucle, pues si el canal no se cierra y se usa en un bucle con `range`, el bucle nunca dejará de esperar nuevos elementos del canal, lo que bloqueará la rutina go actual y hasta más rutinas.
- Ejemplo:
    ```Go
    canal := make(chan int)
    go func() {
        canal <- 1
        canal <- 2
        // No hay close() en el transmisor, por lo que el canal permanece abierto
    }()

    // No sabe que el canal ya no va a enviar elementos y provoca bloqueo de rutinas go
    for valor := range canal {
        fmt.Println(valor)
    }
    ```

### Select

La palabra reservada `select` es básicamente un switch pero de canales, pues permite a una rutina go esperar el resultado de múltiples canales bloqueando su ejecución hasta que alguno de los casos pueda ser ejecutado. Sin embargo, si múltiples casos pueden ser ejecutados al mismo tiempo, se elige uno aleatoriamente.

Además, se puede hacer uso de `default` junto con esta sentencia para poder ejecutar un caso cuando ningún otro caso pueda ser ejecutado y evitar que la rutina actual se bloquee y continue con su ejecución.
- Ejemplo:
    ```Go
    select {
    case <-canal1:
    // Hacer algo porque se recibió algo de canal1
    case <-canal2:
    // Hacer algo porque se recibió algo de canal2
    default:
    // Hacer algo cuando no se reciba nada de canal1 o canal2
    }
    ```

Si no se usa `default`, la rutina go se bloqueará hasta que al menos uno de los casos pueda ejecutarse. `select` evaluará un único caso: si solo uno está listo, ejecutará ese; si varios están listos, elegirá uno aleatoriamente.

# Sección 2: How to Write Go Code

## Organización del código

Go se maneja por paquetes y módulos. Un paquete es una colección de archivos de código que se encuentran en un mismo directorio y se compilan juntos. Por otro lado, un módulo es una colección de paquetes de Go relacionados que se publican juntos como una unidad.

Cada módulo y paquete debe ser identificado de alguna forma. Para esto, existe la **ruta de módulo**, que es un string (nombre) que identifica de forma única al módulo. Mientras que la **ruta de importación** es la ruta que identifica a un paquete dentro de un módulo, formada por la **ruta de módulo** más la ruta del directorio donde se encuentra el paquete dentro del módulo.

Este sistema de identificación es necesario para que Go pueda localizar y manejar correctamente todos los paquetes y módulos. Para gestionar esta información, se utiliza el archivo `go.mod`, que se crea con el comando `go mod init ruta-de-modulo-a-usar`. Este archivo contiene la **ruta de módulo**, la versión de Go requerida, y las dependencias externas del módulo con sus versiones específicas. Por otro lado, comando `go mod tidy` actualiza automáticamente este archivo, agregando las dependencias que sí se usen en el código y eliminando las que ya no sean necesarias.

## Tu primer programa

Go recomienda seguir los siguientes pasos para crear un proyecto simple desde cero:
1. Crear el directorio que contendrá el proyecto
2. Crear el archivo `go.mod` usando el comando `go mod init ruta-de-modulo-a-usar`
3. Crear los archivos que se vayan a usar
    - Se debe tener en cuenta que cualquier comando ejecutable siempre debe usar el paquete main
4. Construir e instalar el proyecto con el comando `go install ruta-de-modulo`
    - Este comando construye el proyecto al crear un archivo binario ejecutable y lo instala dentro de la ruta `$HOME/go/bin/nombre-de-programa`
    - La ruta de instalación depende de las variables `GOPATH` y `GOBIN`
5. Ejecutar el archivo binario como resulte conveniente
    - El nombre del archivo binario ejecutable generado es tomado a partir del identificador del propio módulo

### Importar paquetes del mismo módulo

Algo importante por aclarar, es que en Go hay dos posibles **resultados finales**. Puede ser que se creen archivos binarios ejecutables que utilicen siempre el paquete **main**; o que se creen librerías/paquetes que no utilicen el paquete main ni sean ejecutables directamente, sino que puedan ser utilizados por otros códigos.

Para poder crear y usar un paquete dentro del mismo módulo, se recomienda seguir los siguientes pasos:
1. Crear el directorio que actuará como el paquete dentro del módulo
2. Crear los archivos `.go` con el código del paquete
3. Compilar el paquete con el comando `go build` (opcional para verificación)
    - Este comando no genera ningún archivo de salida visible, simplemente verifica que el paquete compile correctamente y almacena el resultado en el caché local de Go
4. Importar el paquete usando la ruta de importación completa: `import ruta-de-modulo/nombre-de-paquete`

Las funciones, tipos, variables y constantes que empiecen con letra mayúscula son exportadas (públicas) y pueden ser usadas desde otros paquetes. Cualquier otro objeto que empiece con letra minúscula son privadas del paquete y no serán exportadas.

### Importar paquetes de módulos externos

La ruta de módulo puede describir cómo obtener el código de un paquete externo al usar sistemas de control de versiones como **Git**. Go utiliza esta característica para automáticamente obtener los paquetes de repositorios remotos. Una parte importante de esto, es el comando `go mod tidy`. Este comando se encarga de descargar los paquetes externos que se estén usando en el código y grabar su requerimiento y versión en el archivo `go.mod`. Además, elimina cualquier dependencia que no se esté usando en el mismo archivo.

Las dependencias son automáticamente descargadas en el subdirectorio `pkg/mod` del directorio indicado por la variable `GOPATH`. El contenido descargado para una versión específica de un módulo es compartido entre todos los módulos que requieran esa misma versión, por lo que Go marca esos archivos y directorios como **solo-lectura**.

Para remover todas las dependencias descargadas, se puede usar el comando `go clean -modcache`.

## Pruebas

Para hacer pruebas del código, Go ofrece un pequeño framework, para usarlo se necesita el comando `go test` y el paquete estándar `testing`.

Para crear una prueba, se debe crear un archivo con terminación `_test.go` que contenga una función llamada `TestXxx` con la firma `func (t *testing.T)`. La prueba ejecuta la función, y si esta llama a alguna función de error, como `t.Error` o `t.Fail`, se considera que la prueba ha fallado.
- Ejemplo:
```Go
// ./tests/suma_test.go

package tests

import "testing"

func TestSuma(t *testing.T) {
    suma := 2 + 2;
    if suma != 4 {
        // El test falla y muestra el mensaje formateado
        t.Fatalf("%s falló en hacer la suma", t.Name)
    }
}
```

Para ejecutar las pruebas, simplemente se debe estar dentro del directorio donde se encuentran dichas pruebas y usar el comando `go test`.

# Sección 3: The Go Programming Language Specification

## Introducción

Go es un lenguaje de programación de propósito general, es compilado y de tipado estático. Diseñado para ser simple pero poderoso. Go tiene recolección de basura automática, es muy expresivo, maneja programación concurrente, etc. Su idea base es **"menos es más"**, pues deliberadamente no da muchas opciones para hacer una misma tarea, pero las pocas opciones que da son más que suficientes para completarla como se quiere.

## Representación del código fuente

Go representa cada letra en el código fuente como un **código único (code point)** del estándar **Unicode**, y los codifica usando **UTF-8**, por lo tanto, un archivo de código fuente debe ser una secuencia válida de **UTF-8**, por lo que puede trabajar con múltiples lenguajes nativamente.

Esto significa que Go usa **Unicode** para representar cada caracter del código usando **code points**, y luego, usa **UTF-8** para convertir esos códigos en bytes.

## Elementos léxicos

Los elementos léxicos son los **bloques de construcción** más básicos del lenguaje, es decir, son aquellos elementos de Go considerados como las unidades mínimas que el compilador puede reconocer y tomar como válidas.

### Comentarios

Los comentarios sirven como herramienta de documentación del programa dentro del mismo. Existen dos formas en que se pueden usar:
- `//`: Comentarios de una sola línea
- `/**/`: Comentarios de múltiples líneas

Un comentario no puede iniciar dentro de otros elementos como strings, o incluso otros comentarios. Siempre deben estar en su propia línea, antes o después de otros elementos.

### Tokens

Los tokens son básicamente todos los elementos por defecto de todo el vocabulario de Go (no solo palabras reservadas). Se dividen en cuatro clases: **identificatores**, **palabras reservadas**, **operadores y puntuación** y **literales**.

### Punto y coma

En la sintáxis formal y completa de Go sí se usa el punto y coma `;` como finalizador de varias sentencias y producciones. Sin embargo, la mayoría de programas peden omitir su uso siempre y cuando se sigan las siguientes dos reglas:
1. Cuando la sentencia o producción es dividida en múltiples tokens, un punto y coma es automáticamente insertado inmediatamente después del último token
2. Para permitir producciones complejas que ocupen una sola línea, el punto y coma puede ser omitido después de los signos de agrupación terminantes `)` o `}`

### Identificadores

Los identificadores nombran a las entidades del programa, como variables, funciones, tipos, etc. Estos son una secuencia de una o más letras y posibles dígitos, donde el primer caracter del identificador siempre debe ser una letra. Por lo que siempre se debe considerar al crear los si estos deben ser exportados o no.

### Palabras reservadas

Las palabras reservadas son palabras propias del lenguaje y no pueden ser usadas como identificadores, ser modificadas, o cualquier otra cosa diferente a lo establecido.
- `var`
- `const`
- `func`
- `type`
- `package`
- `import`
- `if`
- `else`
- `for`
- `switch`
- `case`
- `default`
- `break`
- `continue`
- `goto`
- `fallthrough`
- `struct`
- `interface`
- `map`
- `chan`
- `go`
- `select`
- `defer`
- `return`
- `range`

### Operadores y puntuación

Existen caracteres o secuencias de caracteres que representan operadores y signos de puntuación.
- `+`
- `-`
- `*`
- `/`
- `%`
- `&`
- `|`
- `^`
- `<<`
- `>>`
- `&^`
- `+=`
- `-=`
- `*=`
- `/=`
- `%=`
- `&=`
- `|=`
- `^=`
- `<<=`
- `>>=`
- `&^=`
- `&&`
- `||`
- `<-`
- `++`
- `--`
- `==`
- `<`
- `>`
- `=`
- `!`
- `~`
- `!=`
- `<=`
- `>=`
- `:=`
- `...`
- `(`
- `[`
- `{`
- `,`
- `.`
- `)`
- `]`
- `}`
- `;`
- `:`

### Enteros literales

Un entero literal es una secuencia de dígitos que representan un valor entero constante. Estos pueden contener un prefijo opcional que establece una base no decimal: `0b` o `0B` para binario; `0`, `0o` o `00` para octal; y `0x` o `0X` para hexadecimal. Además, para mejorar la legibilidad de los dígitos, es posible usar `_` para representar separaciones, pero, debe aparecer únicamente después del prefijo (si existe) o entre los dígitos, no debe estar ni al inicio ni al final del entero literal.

### Puntos-flotantes literales

Un punto flotante literal es una representación decimal o hexadecimal de una constante de punto flotante. Estos se componen de su parte decimal, del punto decimal, y de la parte fraccionaria, incluso pueden contener representación científica mediante el uso de `e` o `E`. Además, igual que los enteros literales, pueden usar `_` para mejorar su legibilidad.

### Imaginarios literales

Un imaginario literal representa la parte imaginaria de una constante compleja. Consiste de un entero o punto flotante seguido por la letra minúscula `i`, por lo que el valor resultante es el valor entero o flotante multiplicado por la unidad imaginaria. Sin embargo, para evitar problemas de compatibilidad, se recomienda usar `0` al inicio.

### Rune literales

Una rune literal representa a una rune constante, es decir, un valor entero que representa un punto de código de Unicode. Estas son expresadas como uno o más caracteres encerrados en comillas simples `'`, y cualquier caracter que aparezca dentro de ellas representa el valor de Unicode correspondiente a dicho caracter.

Una **rune** es el concepto que Go usa para representar un caracter completo. A diferencia, por ejemplo, de `char` en C (que siempre ocupa 1 byte para ASCII), una `rune` puede representar cualquier caracter del estándar Unicode, incluyendo todos aquellos que ocupan de 1 a 4 bytes en UTF-8. Internamente, `rune` es un alias para `int32`, lo que permite representar todo el rango de códigos Unicode.

### String literales

Un string literal representa un string constante obtenido a partir de concatenar una secuencia de caracteres. Existen dos formas de string literales:
- **String literales crudas**: Son una secuencia de caracteres encerrados entre backticks `\``, y cualquier caracter puede aparecer dentro de los mismos (excepto el mismo backtick). El valor de este tipo es un string formado por los caracteres sin interpretar, es decir, no se procesan caracteres especiales, como secuencias de escape
- **String literales interpretados**: Son una secuencia de caracteres encerrados entre comillas dobles `"`, y cualquier caracter puede aparecer dentro de las comillas dobles (excepto una nueva línea y la misma comilla doble, a menos que sean escapados). El valor de este tipo es un string formado por los caracteres interpretados, procesando caracteres especiales como secuencias de escape

## Constantes

Una constante se refiere a un valor cuyo contenido es conocido en tiempo de compilación y nunca cambian de valor a lo largo de la vida del programa. Las constantes en Go pueden ser de tipo booleanas, rune, enteras, punto-flotante, complejas, string, incluso sin tipo. Las constantes sin tipo pueden tomar adaptarse a distintos contextos y tomar el tipo que el contexto determine.

El valor de cualquier constante en Go es representado por alguno de los tipos o alguna expresión/operación constante que pueda ser realizada en tiempo de compilación. Además, el compilador puede implementar las constantes con una precisión interna mayor a la precisión normal en tiempo de ejecución.

## Variables

Una variable es un espacio de memoria para almacenar un valor modificable, y está sujeta completamente a su tipo. Una declaración de una variable reserva un espacio de memoria en tiempo de ejecución que es identificado por el nombre dado a dicha variable (identificador), incluso, se pueden tener espacios de memoria anónimos, que no son accesidos por su identificador, sino por un puntero que contiene su dirección de memoria.

En cuanto a los variables estructuradas (array, slice, struct), estas tienen elementos o miembros a los cuales se les asigna un espacio de memoria individual, por lo que dichos elementos o miembros actúan como variables.

La mayoría de variables tienen un tipo estático, es decir, el tipo que se les asigna en su declaración o de forma implícita. Pero, otras variables de tipo `interface`, pueden tener un tipo dinámico, que es el tipo del objeto que implementa dicha interfaz.

Todas las variables tienen un **valor cero**, el cual es asignado automáticamente si ningún valor (inicializador) es asignado a una variable ya declarada. 

## Tipos

Un tipo determina el conjunto de valores y operaciones que están disponibles para las variables de dicho tipo. Los tipos en Go pueden ser especificados mediante su nombre (tipos nombrados) o mediante su estructura literal (tipos sin nombre).

Los tipos se clasifican en:
* **Predeclarados:** Tipos básicos como `int`, `string`, `bool`, etc., que ya vienen incluidos en el lenguaje
* **Definidos por el usuario:** Nuevos tipos creados mediante declaraciones de tipo usando `type`
* **Tipos literales:** La sintaxis usada para describir tipos compuestos como `[]int`, `map[string]int`, `*Person`

Los tipos se pueden declarar de la siguiente forma:
- **Tipos nombrados:** Se crea un tipo completamente nuevo basado en un tipo predeclarado
    ```Go
    type MyInt int
    ```
- **Alias de tipo:** Se crea un sinónimo para un tipo predeclarado, pero, siguen siendo exactamente el mismo tipo
    ```Go
    type IntAlias = int
    ```

Algunos conceptos clave incluyen el **tipo subyacente**, que es el tipo base de un **tipo nombrado**. También está la **identidad de tipo**, que determina cuándo dos tipos son considerados idénticos, y los **conjuntos de métodos**, que representan el conjunto de métodos disponibles para un tipo.

Una diferencia importante es que los **tipos nombrados** pueden tener sus propios métodos, mientras que los **alias de tipo** heredan los métodos del tipo original y no se les puede agregar métodos nuevos, ya que siguen siendo el mismo tipo.

### Tipo booleano

Un tipo `bool` representa un par de valores booleanos denotados por las constantes predefinidas `true` y `false`.

### Tipo numérico

Existen varios tipos numéricos en Go, como `int`, `float` y `complex`, que representan un conjunto de valores enteros, decimales o complejos, respectivamente. A todos estos se les llama **tipos numéricos**, y los tipos predeclarados independientes de la arquitectura de la máquina son:
- `uint8`: Conjunto de todos los valores sin signo de 8-bits
- `uint16`: Conjunto de todos los valores sin signo de 16-bits
- `uint32`: Conjunto de todos los valores sin signo de 32-bits
- `uint64`: Conjunto de todos los valores sin signo de 64-bits
- `int8`: Conjunto de todos los valores con signo de 8-bits
- `int16`: Conjunto de todos los valores con signo 16-bits
- `int32`: Conjunto de todos los valores con signo 32-bits
- `int64`: Conjunto de todos los valores con signo 64-bits
- `float32`: Conjunto de todos los valores IEEE 754 de 32-bits
- `float64`: Conjunto de todos los valores IEEE 754 de 64-bits
- `complex64`: Conjunto de todos los valores complejos con parte real e imaginaria de tipo float-32
- `complex128`: Conjunto de todos los valores complejos con parte real e imaginaria de tipo float-64
- `byte`: Alias para `uint8`
- `rune`: Alias para `int32`

Además, hay un conjunto de tipos predeclarados cuyo tamaño es específico a la implementación/arquitectura de la máquina:
- `uint`: Puede ser de 32 or 64 bits
- `int`: Puede ser de 32 or 64 bits
- `uintptr`: Un entero sin signo lo suficientemente grande para almacenar un puntero de cualquier tipo

Para evitar problemas de portabilidad, en Go todos los tipos numéricos son definidos, y por lo tanto, específicos a la arquitectura, a excepción de `byte` y `rune`. Además, las conversiones de tipos deben ser explícitas incluso cuando parezcan ser del mismo tamaño.

### Tipo string

El tipo `string` es una secuencia contigua de bytes que representan a cada uno de los caracteres de dicho string, y puede estar vacío. Por lo tanto, el número de bytes usado para representar el string es su longitud y nunca es negativo. Además, los strings son inmutables, por lo que una vez creados no se pueden modificar.

En Go, los caracteres individuales de los strings pueden ser accedidos mediante índices, sin embargo, no es posible obtener la dirección de memoria de dichos elementos individuales. Una cosa importante a tener en cuenta es que la longitud de un string obtenida mediante la función `len()` no representa la cantidad de caracteres del string, sino los bytes utilizados para representar el string, esto debido al uso de Unicode y UTF-8.

### Tipo arreglo

Un arreglo es una secuencia contigua y enumerada de elementos de un único tipo. Este tipo es llamado tipo del elemento, y el número de elementos establece la longitud del arreglo y nunca es negativa. La longitud es parte del arreglo, es decir, que una longitud debe ser asignada al momento de declarar un arreglo, y esta debe evaluar a una constante no negativa de tipo entero.

Los arreglos, a diferencia de C, siempre se trabajan por valor, por lo que siempre se utilizan completos. Incluso, los arreglos son inicializados automáticamente con el valor cero correspondiente al tipo del elemento si no se inicializa manualmente.

Por otro lado, los arreglos `T` no pueden contener elementos del mismo tipo `T` o tipos que contengan elementos del tipo `T` directa o indirectamente, a menos que los tipos que los contienen sean tipos literales (compuestos).

### Tipo slice

Un slice describe un segmento contiguo de un arreglo subyacente y provee acceso a una secuencia de elementos de dicho arreglo, por lo que su tamaño puede ser dinámico. El tipo de elemento del slice siempre debe ser el mismo que el tipo de elemento del arreglo subyacente.

Los slices contienen tres características fundamentales:
- **Arreglo subyacente:** Un puntero que contiene la referencia al primer elemento del segmento del arreglo subyacente al cual tienen acceso
- **Longitud:** El número de elementos del propio slice, y nunca es negativo
- **Capacidad:** El número máximo de elementos del segmento al cual el slice puede acceder del arreglo subyacente

Debido a que los slices trabajan con arreglos subyacentes, múltiples slices pueden usar el mismo arreglo pero diferentes segmentos de él. Por lo tanto, varios slices pueden representar el mismo arreglo; pero varios arreglos no pueden representar el mismo slice.

Un slice puede ser creado usando la función `make()`, la cual siempre crea un nuevo arreglo anónimo utilizado por dicho slice.

### Tipo struct

Una `struct` es una secuencia de elementos nombrados, a los cuales se les conoce como miembros, y cada uno de estos debe tener un nombre y un tipo. Dichos miembros pueden ser nombrados explícitamente o implícitamente, sin embargo, deben ser únicos, a menos que sean miembros vacíos o de relleno.

Un miembro que es declarado con un tipo pero sin un nombre explícitamente, es llamado **tipo embebido**, donde este actúa tanto como tipo como el nombre del miembro. Esto es válido siempre y cuando no se repitan los tipos (nombres).

La declaración de un miembro de cualquier `struct` puede ser seguida de una **etiqueta** opcional, que actúa como un atributo del miembro donde se encuentra la etiqueta. Una etiqueta vacía es lo mismo que una etiqueta ausente. Para poder trabajar con las etiquetas directamente, se necesita el paquete `reflect`.

Por otro lado, los structs `T` no pueden contener elementos del mismo tipo `T` o tipos que contengan elementos del tipo `T` directa o indirectamente, a menos que los tipos que los contienen sean tipos literales (compuestos).

### Tipo puntero

Un tipo puntero permite almacenar la dirección de memoria de una variable de algún tipo específico, donde dicho tipo se convierte en el tipo base del puntero. El valor cero de un puntero es `nil`.

Los punteros en Go utilizan el operador `&` para obtener la dirección de una variable, y el operador `*` para desreferenciar (acceder al valor apuntado). A diferencia de C, Go no permite aritmética de punteros por razones de seguridad, por lo que no se puede incrementar, decrementar o realizar operaciones matemáticas sobre las direcciones de memoria.

Una característica importante es que Go puede detectar casos de desreferenciación de punteros vacíos en tiempo de ejecución, y genera un panic en lugar de comportamiento indefinido.

### Tipo función

Una `func` es un tipo usado para representar a las funciones, donde su valor cero es `nil`.

Las funciones en Go son **ciudadanos de primera clase**, por lo que pueden ser asignadas a variables, ser pasadas como argumentos y ser devueltas por otras funciones. Además, las funciones pueden regresar ninguno o múltiples valores en un mismo retorno, incluso, dichos valores retornados pueden ser nombrados.

Existen también funciones anónimas y funciones variadicas que reciben una cantidad desconocida de parámetros.

### Tipos interfaz

Una `interface` establece comportamiento en lugar de una estructura, por lo que actúa como un contrato que establece comportamientos que otro tipo debe implementar para poder ser implementar la propia interfaz y ser considerado del mismo tipo.

Una variable de tipo interfaz puede almacenar un valor de cualquier tipo que implemente dicha interfaz. Dicho tipo se considerará del tipo interfaz. Por otro lado, el valor cero de un tipo interfaz es `nil`.

Una interfaz es definida por una lista de elementos, donde un elemento puede ser un método (función) u otro elemento de un solo tipo. Su implementación se hace de forma implícita al simplemente implementar los elementos de la interfaz, por lo que no es necesario usar palabras clave ni implementación explícita.

#### Interfaces básicas

Estas son las formas más básicas de una interfaz, donde simplemente se especifica un listado de métodos. Los nombres de dichos métodos deben ser únicos y no estar en blanco. Diferentes tipos pueden implementar las mismas interfaces, incluso, pueden implementar múltiples interfaces al mismo tiempo.

Por otro lado, la interfaz vacía `interface{}` (y su alias `any`) puede contener cualquier tipo, incluso otras interfaces pueden ser asignadas a la interfaz vacía.

#### Interfaces embebidas

Estas son formas un poco más generales de una interfaz, donde una interfaz puede embeber o incluir otras interfaces dentro de su lista de elementos. Esto permite crear composición de comportamientos al combinar múltiples interfaces en una sola.

Cuando una interfaz embebe otras interfaces, un tipo debe implementar todos los métodos de todas las interfaces embebidas para satisfacer la propia interfaz compuesta. Si diferentes interfaces embebidas contienen métodos con el mismo nombre, estos deben tener la misma firma (mismos parámetros y valores de retorno) para evitar conflictos.

Las interfaces embebidas facilitan la composición y reutilización de comportamientos, permitiendo construir interfaces más complejas a partir de interfaces más simples y específicas.

#### Interfaces genéricas

Estas son las formas más generales de una interfaz, donde una interfaz puede contener elementos de tipo arbitrario `T` (genérico) o tipos `~T` que contengan un tipo `T` subyacente. Junto con métodos con tipos de parámetro arbitrario, permiten definición genérica y reutilización de código para múltiples tipos.

Las interfaces más genéricas pueden especificar diferentes restricciones de tipo usando:
- **Tipos exactos:** `T` acepta solo el tipo `T`
- **Tipos subyacentes:** `~T` acepta cualquier tipo con tipo subyacente `T`
- **Tipos unión:** `T1 | T2` acepta `T1` o `T2` pero no ambos al mismo tiempo
- **Combinaciones:** `~T1 | ~T2` acepta cualquier tipo con tipo subyacente `T1` o `T2` pero no ambos al mismo tiempo

**Limitaciones importantes:**

- Una interfaz genérica que contiene restricciones de tipo no puede ser usada como tipo de variable ordinaria, solo como restricciones de tipo en funciones o tipos genéricos
- Las restricciones de tipo y los métodos pueden combinarse en la misma interfaz
- Las interfaces genéricas pueden embeberse en otras interfaces genéricas

### Tipo mapa

Un `map` es un grupo de elementos en la forma **llave-valor** sin un orden específico. Todos los **valores** deben ser de un mismo tipo, y están indexados por sus **llaves** correspondientes, que también deben ser de un mismo tipo. Formando así un conjunto de elementos **llave-valor**.

El valor de un mapa sin inicializar es `nil`, y no es posible agregar contenido. Pero, un mapa sin inicialiazar es diferente a un mapa vacío, pues en un mapa vacío sí es posible agregar contenido nuevo. Por otro lado, el tipo de la llave debe poder ser comparable y tener bien definidos los operadores de comparación `==` y `!=`, por lo que las llaves no pueden ser de tipo función, mapa, slice, etc.

El número de elementos de un mapa es conocido como su **longitud** y puede ser obtenida usando la función `len()`. Además, un mapa puede ser creado con la función `make()` que recibe el mapa a crear y su capacidad inicial opcional, aunque dicha capacidad no es fija y no limita al propio mapa.

### Tipo canal

Un `chan` proporciona un mecanismo para permitir la comunicación sincronizada entre múltiples **rutinas go**, para todas las operaciones de enviar y recibir valores de un tipo específico. El valor de un canal sin inicializar es `nil`.

Para trabajar con los canales se debe utilizar el operador `<-`, pues este especifica la dirección del canal, ya sea para enviar o para recibir. Si se provee una dirección específica al momento de crear un canal, dicho canal tendrá únicamente esa dirección, pero, si no se proporciona ningua dirección se considerará como un canal bidireccional. Por lo tanto, dependiendo de la dirección proporcionada, los canales pueden ser limitados a solo recibir o enviar.

Los canales se pueden crear usando la función `make()`, donde se recibe el canal a crear y opcionalmente la capacidad (buffer) del canal. Si no se especifica la capacidad o es igual a 0, se crea un canal sin capacidad (unbuffered). También, se puede usar la función `close()` para cerrar un canal. Un canal puede ser usado en múltiples funciones concurrentes sin necesidad de sincronización, pues la propia naturaleza de los canales permite este comportamiento.

Cabe mencionar que un **canal sin buffer** solo puede ser usado cuando ambas partes de la comunicación estén listas, es decir, cuando existe un emisor y un receptor. Mientras que un **canal con buffer** puede estar constantemente recibiendo y enviando valores, siempre y cuando no esté lleno o vacío, respectivamente. Además, funcionan usando el concepto FIFO (First-In, First-Out).

## Propiedades de tipos y valores

### Representación de valores

Todos los valores de los tipos predeclarados, arreglos y structs contienen su propia información almacenada directamente en ellos mismos, es decir, que se utilizan por valor. Cuando se asignan o pasan como argumentos, siempre se crea una copia completa de toda su información, la cual es almacenada directamente en el parámetro o variable al cual están siendo asignados.

Por otro lado, tipos como punteros, funciones, slices, mapas y canales se utilizan por referencia y almacenan metadatos que referencían a su información subyacente. Por ejemplo, un slice no solo contiene una referencia a su arreglo subyacente, sino también metadatos como longitud y capacidad. Esto permite que múltiples variables puedan referenciar la misma información subyacente pero con diferentes metadatos.

El tipo interfaz tiene un comportamiento dinámico en cuanto a su representación, ya que su valor puede ser autocontenido o referenciado, dependiendo del tipo dinámico de la interfaz, es decir, del tipo concreto que implementa la interfaz en tiempo de ejecución.

Una consecuencia importante de esta distinción es que los tipos que se usan por valor siempre tienen un valor cero diferente a `nil`, mientras que el valor cero de los tipos que se usan por referencia siempre es `nil`.

### Tipos subyacentes

Todos los tipos en Go tienen un tipo subyacente que define su estructura fundamental y representación en memoria.

Para tipos predeclarados (como `int`, `string`, `bool`), el tipo subyacente es el mismo tipo en sí, por ejemplo, el tipo subyacente de `int` es `int`. Para tipos compuestos construidos con tipos literales (como `[]int`, `map[string]int`, `chan bool`), el tipo subyacente es la estructura del tipo literal mismo. Es importante mencionar que incluso si dos tipos diferentes usan el mismo tipo subyacente, siguen siendo dos tipos completamente diferentes, a menos que sean declarados como alias.

De forma resumida, el tipo subyacente aplica a todos los tipos individualmente y determina la forma en que se va a representar dicho tipo en la memoria y las operaciones básicas permitidas.

### Tipos base

Todos los tipos que no son interfaces tienen un tipo base, el cual es idéntico a su tipo subyacente.

Las interfaces tienen un comportamiento especial para determinar su tipo base, pues una interfaz tiene un tipo base únicamente si se cumple alguna de estas condiciones:
1. Todos los tipos en el conjunto de tipos de la interfaz comparten el mismo tipo subyacente `T`, y al menos uno de esos tipos no es una interfaz. En este caso, el tipo base de la interfaz es el tipo `T`
2. Todos los tipos en el conjunto de tipos de la interfaz son de tipo canal con el mismo tipo de elemento y la misma dirección (enviar, recibir, o bidireccional)

Si una interfaz no cumple alguna de estas condiciones, no tiene tipo base, y por definición nunca puede ser un tipo definido, creado o de tipo interfaz.

De forma resumida, el tipo base aplica o está diseñado principalmente para las interfaces usadas de forma genérica y garantiza que todos los tipos en el conjunto de tipo de dichas interfaces permitan realizar las mismas operaciones.

### Identidad del tipo

Esta propiedad se refiere a cuándo es que dos tipos son considerados exactamente el mismo tipo por el compilador de Go, determinando así, si comparten características y comportamientos idénticos.

Un tipo definido por el programador (tipo nombrado como `type MyInt int`) siempre es diferente a cualquier otro tipo, incluso si tienen el mismo tipo subyacente.

Para tipos no-definidos (tipos literales), dos tipos son idénticos si sus estructuras son completamente equivalentes en todos los aspectos:
- **Tipos arreglo:** Idénticos si el tipo de elementos es idéntico y tienen la misma longitud
- **Tipos slice:** Idénticos si el tipo de elementos es idéntico
- **Tipos struct:** Idénticos si tienen la misma secuencia de campos con nombres, tipos, etiquetas idénticas, y el mismo estado de tipos embebidos
- **Tipos puntero:** Idénticos si apuntan a tipos idénticos
- **Tipos función:** Idénticos si tienen igual número de parámetros y resultados con tipos idénticos, y ambas son variádicas o ninguna lo es
- **Tipos interfaz:** Idénticos si definen exactamente el mismo conjunto de tipos (métodos y campos)
- **Tipos mapa:** Idénticos si los tipos de llaves y valores son idénticos
- **Tipos canal:** Idénticos si el tipo de elementos es idéntico y tienen la misma direccionalidad

Que dos tipos sean idénticos quiere decir que esos tipos son iguales en todos sus aspectos individuales relevantes para el compilador. Entonces, la -*identidad del tipo** implica que dichos tipos puedan ser tratados de la misma forma y no necesiten conversiones explícitas.

### Asignabilidad

Esta propiedad determina cuándo el valor `x` de tipo `V` puede ser asignado a una variable de tipo `T`, incluso cuando los tipos no son idénticos. Esta flexibilidad permite mayor interoperabilidad en el sistema de tipos de Go.

Un valor es asignable cuando se cumple alguna de estas condiciones:
- `V` y `T` son tipos idénticos (caso más directo)
- `V` y `T` tienen tipos subyacentes idénticos, donde ninguno es un tipo genérico y al menos uno no es un tipo nombrado
- `V` y `T` son tipos canal con tipos de elementos idénticos, donde `V` es bidireccional y al menos uno no es un tipo nombrado
- `T` es un tipo interfaz (no genérico) y el valor `x` implementa `T` (está en el conjunto de tipos de `T`)
- `x` es el valor `nil` y `T` es un tipo que usa referencias (puntero, función, slice, mapa, canal, interfaz) y no es un tipo genérico
- `x` es una constante sin tipo que puede ser representada por el tipo `T`

### Representabilidad

Esta propiedad se aplica específicamente a constantes y determina si una constante `x` puede ser correctamente almacenada y representada como valor de un tipo `T` (donde `T` no es un tipo genérico).

Una constante `x` es representable por tipo un tipo `T` cuando se cumple alguna de estas condiciones:
- `x` está dentro del rango de valores que `T` puede representar
- `T` es un tipo de punto-flotante y `x` puede ser redondeado a la precisión de `T` sin desbordamiento
- `T` es un tipo complejo y tanto la parte real como imaginaria de `x` son individualmente representables por el tipo de subyacente de `T` que representa ambas partes

Básicamente esta propiedad aplica para las constantes sin tipo que determina si dicha constante puede ser asignada a una variable de cierto tipo sin causar errores de compilación o pérdida de información crítica.

### Conjunto de métodos

El conjunto de métodos de un tipo determina qué métodos pueden ser llamados desde instancias de ese tipo o directamente desde el tipo y, crucialmente, qué interfaces puede implementar el tipo.

**Reglas fundamentales:**
- **Para un tipo definido T:** El conjunto de métodos incluye todos los métodos declarados con argumento receiver de valor `(t T)`
- **Para un tipo puntero \*T:** El conjunto de métodos incluye todos los métodos declarados con argumento receiver de valor `(t T)` y receiver de pointer `(t \*T)`
- **Para un tipo interfaz:** El conjunto de métodos de un tipo interfaz es la intersección del conjunto de métodos de cada elementos de la interfaz, es decir, solo los métodos que todos los elementos tienen
- **Para tipos embebidos en structs:** Los métodos del tipo embedded se promueven al conjunto de métodos del struct contenedor

Un tipo `T` implementa una interfaz `I` solo si el conjunto de métodos de `T` contiene todos los métodos requeridos por `I`. Además, todos los tipos tienen conjunto de métodos (aunque puede estar vacío), y todos los métodos deben tener un nombre único y no estar en blanco.

## Bloques

Un bloque es una secuencia (posiblemente vacía) de declaraciones y sentencias encerradas dentro de llaves `{}`.

Los bloques explícitos son aquellos delimitados por llaves visibles en el código, pero también existen bloques implícitos que no requieren llaves:
- **Bloque universal:** Engloba todo el código fuente de Go y contiene todas las declaraciones predefinidas (`int`, `string`, `nil`, `true`, etc.)
- **Bloque de paquete:** Engloba todo el código fuente dentro de un paquete específico
- **Bloque de archivo:** Engloba todo el código fuente dentro de un archivo individual
- **Bloque de función:** Cada función o método crea su propio bloque
- **Bloque de sentencia:** Estructuras de control (`if`, `for`, `switch`, etc.) y bloques explícitos `{}` crean sus propios bloques

Los bloques forman una jerarquía anidada donde cada bloque interno puede acceder a declaraciones de bloques externos, pero no viceversa. Las declaraciones en bloques internos pueden llegar a ocultar (shawdowing) declaraciones de bloques externos que tengan el mismo nombre. Esta estructura determina la visibilidad y duración de variables, constantes, tipos y funciones en Go.

## Declaraciones y alcance

Una declaración relaciona un identificador (que no esté en blanco) con algún objeto de Go, como `const`, `type`, `type parameter`, `var`, `func`, `label` o `package`. Cualquier identificador usado debe ser declarado y no estar en blanco, además, no se puede declarar el mismo identificador en el mismo bloque. Los identificadores a nivel paquete no pueden redeclararse.

El identificador en blanco `_` puede usarse como cualquier otro identificador en una declaración, pero no establece ninguna relación (no es realmente declarado), permitiendo descartar valores.

**Reglas de scope (Go usa lexical scoping con bloques):**
1. **Identificadores predeclarados:** Alcanzan el bloque universal
2. **Constantes, tipos, variables, o funciones (pero no métodos)**: Alcanzan el bloque de paquete
3. **Nombres de paquetes importados:** Alcanzan el bloque del archivo que contiene la declaración de import
4. **Parámetro receiver, parámetros de función, o variables de resultado:** Alcanzan el bloque de función donde están declarados
5. **tipos de parámetro de funciones o parámetros receivers:** Su alcance inicia después del nombre de la función y termina al final del cuerpo de la función donde están declarados
6. **tipos de parámetro:** Su alcance inicia después del nombre del tipo y termina al final de la declaración
7. **Constantes o variables declarados dentro funciones:** Su alcance inicia al final de la declaración y termina al final del bloque contenedor más interno
8. **Tipos declarados dentro de funciones:** Su alcance inicia al final de la declaración y termina al final del bloque contenedor más interno

Un identificador declarado en un bloque interno puede ocultar uno del bloque exterior con el mismo nombre (shadowing). Por otro lado, la palabra reservada `package` no es una declaración, sino una directiva que identifica archivos del mismo paquete y especifica el nombre por defecto al importar.

### Alcance de etiquetas

Las etiquetas son declaradas mediante el uso de `:` y son usadas automáticamente en las declaraciones de `break`, `continue` y `goto`. Una etiqueta declarada siempre debe ser usada, pues no está permitido declararla sin ser usada.

A diferencia de otros identificadores, las etiquetas tienen un alcance único limitado a la función en la que se declaran y no interfieren con otros identificadores que tengan el mismo nombre (pueden coexistir sin conflicto).

### Identificador en blanco

El identificador en blanco es representado por el caracter `_`. Sirve como un placeholder anónimo en lugar de un identificador normal, y puede usarse múltiples veces en el mismo scope sin causar conflictos de redeclaración.

### Identificadores predeclarados

Hay un total de 44 identificadores predeclarados en el bloque universal de Go. Estos sí son modificables, a diferencia de las palabras reservadas, pero NO es recomendable hacerlo.

**Tipos:**
- `any`
- `bool`
- `byte
- `comparable`
- `complex64`
- `complex128`
- `error`
- `float32`
- `float64`
- `int`
- `int8`
- `int16`
- `int32`
- `int64`
- `rune`
- `string`
- `uint`
- `uint8`
- `uint16`
- `uint32`
- `uint64`
- ``uintptr`

**Constantes:**
- `true`
- `false`
- `iota`

**Valor cero:**
- `nil`

**Funciones:**
- `append`
- `cap`
- `clear`
- `close`
- `complex`
- `copy`
- `delete`
- `imag`
- `len`
- `make`
- `max`
- `min`
- `new`
- `panic`
- `print`
- `println`
- `real`
- `recover`

### Identificadores exportados

Un identificador puede ser exportado para permitir acceso desde otros paquetes. Un identificador es exportado únicamente cuando cumple dos condiciones:
- El primer caracter es una letra mayúscula representable por el estándar Unicode
- El identificador es declarado en el bloque de paquete o corresponde a un miembro de un struct o es un método

Los identificadores que no cumplan estas dos condiciones no son exportados y solo pueden usarse dentro del mismo paquete donde se declaran.

### Unicidad de los identificadores

En un conjunto de identificadores, un identificador es único cuando es diferente a cualquier otro identificador de ese conjunto.

**Dos identificadores son diferentes si:**
- Se escriben diferente (case-sensitive)
- Están en paquetes diferentes
- Están en el mismo paquete pero no son exportados (limitados al alcance de su propio paquete)

**Dos identificadores son iguales si:**
- Tienen la misma escritura y están en el mismo contexto accesible (mismo paquete o ambos exportados)

### Declaración de constantes

Una declaración de constantes relaciona una lista de identificadores con una lista de valores dados por expresiones constantes. La cantidad de identificadores debe coincidir con la cantidad de expresiones.

- **Con tipo explícito:** Si se especifica un tipo, todas las constantes adoptan ese tipo y sus expresiones deben ser asignables a él

- **Sin tipo explícito:** Cada constante adopta el tipo individual correspondiente a su expresión respectiva
- **Declaraciones agrupadas:** En declaraciones múltiples dentro de paréntesis, es posible omitir valores en las declaraciones posteriores, pues automáticamente reutilizan el valor y tipo de la declaración anterior

**ConstSpec:** Es un término técnico que simplemente se refiere una línea individual donde se declara una constante

### Iota

El identificador predeclarado `iota` representa una secuencia numérica entera sin tipo para generar constantes automáticamente.

**Funcionamiento:**
- Su valor corresponde al índice de la línea donde se hace la declaración, iniciando en 0
- Se incrementa automáticamente en cada nueva línea de declaración
- Se resetea a 0 en cada nueva agrupación de declaración de constantes (`const`)

**Comportamiento especial:** Múltiples usos de `iota` en el la misma línea representan el mismo valor (no se incrementa dentro de la misma línea)

### Declaraciones de tipo

Una declaración de tipo relaciona un identificador (nombre del tipo) con un tipo nuevo o existente. Las declaraciones pueden ser de dos formas: declaraciones de alias o definiciones de tipos completamente nuevos.

#### Declaración de alias

La declaración de alias (e.g. `type NuevoNombre = TipoPredeclarado`) relaciona un identificador con un tipo predeclarado. Por lo tanto, no crea un nuevo tipo, simplemente establece una forma alternativa de referenciar el mismo tipo, siendo tratados como idénticos.

Los alias funcionan de acuerdo a su alcance. Pueden usar tipos de parámetro creando **alias genéricos**, los cuales deben ser instanciados al usarse.

#### Definición de tipos

La definición de tipos (e.g. `type NuevoTipo TipoPredeclarado`) relaciona un identificador con un tipo completamente nuevo. Crea un **tipo nombrado** que usa un tipo existente como tipo subyacente.

**Características de tipos nombrados:**
- Son diferentes a cualquier otro tipo, incluyendo su tipo base
- Pueden tener métodos propios asociados
- No heredan métodos del tipo base
- Pueden ser tipos genéricos que usen tipos de parámetro

Para los tipos genéricos, los métodos asociados deben declarar la misma cantidad de tipos de parámetro que el tipo definido.

### Declaración de tipos de parámetro

Una lista de tipos de parámetro declara los tipos genéricos para funciones genéricas o declaraciones de tipos. Su estructura es similar a parámetros regulares, pero están encerrados en corchetes `[]` e inmediatamente después del nombre de la función/tipo y antes de sus parámetros regulares.

Todos los nombres de los tipos de parámetro en la lista que no estén en blanco deben ser únicos. Estos actúan como tipos nombrados temporales que sirven como placeholders, los cuales son reemplazados por tipos concretos duranta la instanciación.

Cada tipo de parámetro tiene una restricción de tipo correspondiente que define sus restricciones.

#### Restricciones de tipo

Un restricción de tipo es una interfaz que define el conjunto de tipos permitidos (conjunto de tipos) para un tipo de parámetro y controla las operaciones disponibles sobre valores de esos tipos.

#### Cumplimiento de las restricciones de tipo

Un tipo cumple con una restricción de tipo cuando:
- Implementa la interfaz de la restricción (tiene los métodos requeridos), o
- está incluido en el conjunto de tipos de la restricción (listado explícitamente con `|`)

### Declaración de variables

La declaración de variables con la palabra reservada `var` puede crear una o más variables, relacionando identificadores con tipos específicos y valores iniciales opcionales. Cuando hay una lista de expresiones, las variables se inicializan con sus valores correspondientes, pero si no se provee inicializador, se asigna el valor cero del tipo. El tipo puede especificarse explícitamente o ser omitido, en cuyo caso la variable adopta el tipo inferido de la expresión de inicialización.

### Declaración corta de variables

La declaración corta usa el operador `:=` sin necesidad de `var` ni tipo explícito. Solo está permitida dentro de funciones (no a nivel de paquete) y siempre requiere un inicializador. En asignaciones múltiples, puede redeclarar variables existentes siempre que al menos una variable sea nueva en ese bloque.

### Declaración de funciones

La declaración de una función con `func` relaciona un identificador con una función. Una función tiene una firma específica (parámetros y valores de retorno) y debe seguir las reglas del lenguaje, como terminar con una expresión de retorno si declara valores de retorno, o manejar todos los casos de ejecución apropiadamente.

### Declaración de métodos

Un método es una función con un parámetro receiver, lo que significa que está asociada específicamente al tipo declarado en su receiver. La declaración de método relaciona un identificador con un método y lo asocia al tipo del receiver correspondiente.

El receiver se declara después de `func` pero antes del nombre del método, debe ser un parámetro único no variadico cuyo tipo se esté definido por valor o por referencia (llamado tipo base del receiver). El identificador del receiver no puede estar en blanco y debe ser único dentro de toda la firma del método. Los métodos con receiver de valor vs receiver de puntero tienen diferentes conjuntos de métodos, lo que afecta qué interfaces pueden implementar.

## Expresiones

Una expresión especifica la computación a realizar aplicando operadores y funciones a valores (operandos).

### Operandos

Los operandos representan los valores elementales usados en expresiones. Pueden ser identificadores que representen constantes, variables o funciones, o expresiones anidadas entre paréntesis. 

El identificador en blanco `_` solo puede usarse en el lado izquierdo de asignaciones para descartar valores.

### Identificadores calificados

Un identificador calificado accede a identificadores exportados de otros paquetes usando la sintaxis `paquete.Identificador`. Tanto el nombre del paquete como el identificador deben ser diferentes al identificador en blanco, y el identificador debe estar exportado (empezar con mayúscula) para ser accesible desde el paquete importador.

### Literales compuestos

Los literales compuestos construyen valores para tipos compuestos (structs, arreglos, slices, mapas) usando la sintaxis `Type{elements}`. Cada evaluación crea una nueva instancia.

La estructura de los elementos varía según el tipo: los structs pueden usar nombres de campos, los arreglos pueden especificar índices, etc. Para tipo de parámetros, todos los tipos en su conjunto de tipos deben ser válidos para literales compuestos para poder usarlos.

### Funciones literales

Una función literal representa una función anónima que no puede declarar tipos de parámetros. Puede ser asignada a variables o invocada directamente. Este tipo de funciones son son closures, lo que significa que pueden capturar y usar variables de alcance externo a donde se definen. Estas variables capturadas son compartidas entre la función externa y el closure, manteniéndose vivas mientras el closure exista.

### Expresiones primarias

Las expresiones primarias son los operandos fundamentales para construir expresiones más complejas (unarias y binarias). Incluyen identificadores, literales, expresiones entre paréntesis, y expresiones que acceden a elementos o campos.

### Selectores

Un selector (`expresion.selector`) accede a un campo o método de un valor. La expresión debe ser primaria y no puede ser un nombre de paquete. Los selectores funcionan automáticamente tanto con valores directos como con punteros, pues Go maneja implícitamente la dereferenciación cuando es necesario.

### Expresiones de métodos

Una expresión de método es una forma de referenciar un método de un tipo como si fuera una función regular, donde el receiver se convierte en el primer parámetro explícito de la función.

Cuando se define un método con la sintaxis `func (t T) Metodo(args) TipoRetorno { ... }`, se puede crear una expresión de método usando `T.Metodo`. Esta expresión resulta en una función que tiene la firma `func(t T, args) TipoRetorno`, donde el receiver original ahora es el primer parámetro explícito.

Las expresiones de métodos se diferencían de los valores de métodos. Una expresión de método como `T.Metodo` requiere que se pase la instancia como primer argumento cuando es llamada. Por el otro lado, un valor de método como `instancia.Metodo` ya tiene la instancia *capturada* y no necesita que se le pase explícitamente.

En cuanto a las reglas para crear expresiones de métodos, solo se pueden crear desde el tipo que está en el conjunto de métodos correspondiente. Los métodos con receivers por valor `(t T)` permiten la sintaxis `T.Metodo`. Sin embargo, los métodos con receivers por puntero `(t *T)` únicamente permiten `(*T).Method`, ya que estos métodos no forman parte del conjunto de métodos del tipo valor.

### Valores de métodos

Un valor de método es una forma de referenciar un método desde una instancia específica, donde el receiver queda *capturado* dentro de la función resultante.

Cuando se tiene una instancia y se referencía uno de sus métodos usando `instancia.Metodo` (sin paréntesis), se obtiene una función que ya no requiere el receiver como parámetro. Si el método original tiene la firma `func(t T) Metodo(args) TipoRetorno`, el valor de método resultante tiene la firma `func(args) TipoRetorno`.

A diferencia de las expresiones de método, los valores de método pueden crearse desde cualquier instancia, independientemente del tipo de receiver del método. Go realiza automáticamente las conversiones necesarias entre `T` y `*T` cuando se crea el valor de método, permitiendo que tanto valores como punteros puedan generarlos para métodos con cualquier tipo de receiver.

### Expresiones de índice

Una expresión primaria en la forma `a[x]` representa un elemento de un arreglo, slice, string o mapa donde `x` es su índice o posición (para arreglos, slices y strings), o clave (para mapas).

**Para arrays, slices y strings**  
El índice debe ser una constante sin tipo o un valor de tipo `int`. Debe ser un número no negativo representable por el tipo `int`, y debe estar en el rango `0 <= índice < len(objeto)`. Una constante sin tipo usada como índice toma automáticamente el tipo `int`. Si el índice está fuera del rango permitido, se produce un panic en tiempo de ejecución.
- **Arreglos:** `a[x]` representa el elemento en el índice `x` del arreglo `a`. El comportamiento es el mismo tanto si se usa un arreglo directamente como un puntero a un arreglo
- **Slices:** `a[x]` representa el elemento en el índice `x` del slice `a`
- **Strings:** `a[x]` representa el byte en el índice `x` del string `a`. Para strings, el índice debe ser una constante entera, y el resultado no puede ser asignado (los strings son inmutables)

**Para mapas**  
El índice `x` debe ser asignable al tipo de las claves del mapa. Si el mapa contiene `x` como clave, se devuelve el valor correspondiente. Si el mapa no contiene la clave, se devuelve el valor cero del tipo de valores del mapa.

**Para tipos de parámetro**  
La expresión de índice `a[x]` debe ser válida para todos los tipos del conjunto de tipos del tipo de parámetro. Esto significa que todos los tipos en el conjunto de tipos deben soportar la operación de indexado con el tipo de `x`.

Para cualquier otro tipo que no sea arreglo, slice, string, mapa o tipo de parámetro, el uso de expresiones de índice no está permitido.

### Expresiones de slice

Las expresiones de slice construyen un substring o un slice a partir de un string, arreglo, puntero a un arreglo o slice. Existen dos variantes: una forma simple que especifica un rango (inicio y fin), y una forma completa que también especifica la capacidad del slice resultante.

Para tipos de parámetro, a menos que todo su conjunto de tipos contenga únicamente strings, el tipo de elemento de todos los tipos en el conjunto debe ser el mismo.

#### Expresiones de slice simples

Este tipo de expresiones utilizan la sintaxis `a[bajo:alto]` para especificar un rango de elementos. El índice inferior (`bajo`) es inclusivo, mientras que el índice superior (`alto`) es exclusivo.

Cualquiera de los dos índices puede ser omitido por conveniencia. Si se omite el índice inferior, toma el valor `0`. Si se omite el índice superior, toma el valor de la longitud del objeto (`len(objeto)`).

Los índices deben ser enteros no negativos. Para strings y arreglos, deben cumplir `0 <= bajo <= alto <= len(objeto)`. Para slices, el índice superior puede extenderse hasta la capacidad del slice: `0 <= bajo <= alto <= cap(slice)`.

Si la expresión de slice es válida pero el objeto del cual se obtiene el slice es inválido, el resultado es `nil`. Todos los slices generados a partir del mismo objeto subyacente comparten el mismo arreglo subyacente.

#### Expresiones de slice completas

Las expresiones de slice completas utilizan la sintaxis `a[bajo:alto:maximo]` y están disponibles para arreglos, punteros a un arreglo y slices, pero no para strings. El tercer índice (`max`) controla la capacidad del slice resultante.

Los índices `bajo` y `alto` funcionan igual que en las expresiones de slice simples. El índice `maximo` establece que la capacidad del slice resultante será `maximo - bajo`. Solo el primer índice (`bajo`) puede ser omitido, tomando el valor `0`.

Los índices deben cumplir `0 <= bajo <= alto <= maximo <= cap(objeto)` y ser enteros no negativos.

### Aserción de tipos

Una aserción de tipo es una expresión de la forma `x.(T)` que verifica que `x` no es `nil` y que el valor almacenado en `x` es del tipo `T`. Esta operación solo es válida cuando `x` es de tipo interfaz.

**Comportamiento según el tipo T**  
- Si `T` no es un tipo interfaz, la aserción de tipo verifica que el tipo dinámico de `x` sea idéntico a `T`
- Si `T` es un tipo interfaz, la aserción de tipo verifica que el tipo dinámico de `x` implemente la interfaz `T`

Si la aserción de tipo es válida, la expresión devuelve el valor almacenado en `x` convertido al tipo `T`. Pero, si es inválida, se produce un pánico en tiempo de ejecución. Para evitar el pánico, se puede usar la forma de dos valores: `valor, ok := x.(T)`. En esta variante, si la aserción es válida, `valor` contiene el valor convertido y `ok` es `true`. Si es inválida, `valor` es el valor cero del tipo `T` y `ok` es `false`.

### Expresión de llamadas

Una expresión de llamada con la sintaxis `f(a1, a2, ..., an)` invoca a la función `f` con los argumentos especificados. Excepto en un caso especial, todos los argumentos deben ser asignables a los tipos de sus parámetros correspondientes.

**Evaluación y orden de ejecución**  
Los argumentos son evaluados antes de realizar la llamada a la función. Durante la llamada, el valor de la función y sus argumentos se evalúan en orden normal. Posteriormente, se reserva espacio en memoria para las variables de la función (parámetros, valores de retorno y variables locales). Los argumentos se asignan a los parámetros correspondientes y comienza la ejecución de la función.

**Diferencia entre métodos y funciones**  
Un método se invoca directamente desde un tipo o una instancia del mismo (por ejemplo, `instancia.Metodo()` o `Tipo.Metodo()`), mientras que una función se llama de forma independiente o mediante un identificador calificado (por ejemplo, `fmt.Println()`).

Llamar a una función `nil` produce un pánico en tiempo de ejecución.

Para funciones genéricas, deben ser instanciadas antes de poder ser llamadas o utilizadas como valores. Si el tipo de la función es un tipo de parámetro, todos los tipos en su conjunto de tipos deben tener el mismo tipo subyacente (tipo función).

### Pasando argumentos a parámetros "..."

Una función es variádica (cantidad de parámetros variantes) cuando su último (o único) parámetro tiene la forma `...T`, donde `T` es el tipo de los elementos. Dentro de la función, este parámetro se comporta como un slice de tipo `[]T`.

Si no se pasan argumentos para el parámetro variádico, su valor es `nil`. Si se pasan uno o más argumentos, el parámetro recibe un slice cuyos elementos son los argumentos proporcionados. La longitud y capacidad de este slice corresponden exactamente al número de argumentos pasados.

Cuando el argumento final en una llamada a una función variádica es un slice del tipo correspondiente seguido por `...`, ese slice se pasa directamente sin modificaciones. En este caso, no se crea un nuevo slice dentro de la función, por lo que, tanto quien llama a la función, como la propia función comparten el mismo arreglo subyacente. Esta característica permite optimizar las llamadas variádicas cuando ya se tiene un slice disponible, evitando copias innecesarias de datos.

### Instanciaciones

Una función o tipo genérico es instanciado al sustituir los tipos de parámetro por tipos de argumento específicos. Este proceso convierte una declaración genérica en una versión concreta no genérica.

La instanciación se realiza en dos pasos secuenciales:
1. **Sustitución:** Cada tipo de argumento reemplaza a su correspondiente tipo de parámetro en toda la declaración genérica. Esta sustitución ocurre en la función o tipo completo, incluyendo la lista de tipos de parámetros y cualquier referencia a tipos en la declaración
2. **Verificación de restricciones:** Después de la sustitución, cada tipo de argumento debe satisfacer las restricciones del tipo de parámetro correspondiente. Si algún tipo de argumento no cumple con sus restricciones, la instanciación falla

Instanciar un tipo genérico resulta en un nuevo tipo nombrado no genérico. Instanciar una función genérica produce una nueva función no genérica.

Para funciones genéricas, los tipo de argumentos pueden especificarse explícitamente (recomendado) o pueden ser parcial o totalmente omitidos, cuando se omiten, Go realizará inferencia de tipo basándose en el contexto de uso. Para tipos genéricos, los tipos de argumento deben ser especificados explícitamente en todos los casos, pues Go no realiza inferencia de tipos para la instanciación de tipos genéricos.

### Inferencia de tipos

Al usar una función genérica, es posible omitir algunos o todos los tipos de argumentos siempre y cuando puedan ser inferidos desde el contexto de uso, considerando las restricciones de los tipos de parámetros correspondientes.

La inferencia de tipos funciona mediante las relaciones que existen entre pares de tipos. Un argumento debe ser asignable a su parámetro correspondiente, lo que crea una relación entre ambos tipos. Si alguno de estos tipos contiene tipos de parámetro, Go se asegura de que los tipos de argumento sean asignables y satisfagan las restricciones de su respectiva relación.

Cada par de tipos correspondientes forma una **ecuación de tipo** que contiene uno o múltiples tipo de parámetros de una o múltiples funciones genéricas. Los tipos de parámetros que necesitan ser resueltos (aquellos cuyos tipos de argumentos no fueron proporcionados explícitamente) se denominan **tipos de parámetros limitantes**. Un argumento puede contener otra función genérica, ampliando el conjunto de parámetros de tipo limitantes a resolver cuando sus tipos de argumentos tampoco se proporcionan.

La inferencia de tipos prioriza la información obtenida directamente de los operandos antes que los valores específicos, y ocurre en dos fases:
1. Las ecuaciones de tipo se resuelven para los parámetros de tipo limitantes usando unificación de tipos. Este proceso identifica qué tipos deben tener los tipos de parámetros basándose en los argumentos proporcionados directamente. Si esta fase falla, la inferencia completa falla
2. Para cada tipo de parámetro limitante que no pudo ser inferido en la primera fase, Go examina información adicional como tipos de retorno de funciones pasadas como argumentos, signatures completas de funciones, y restricciones que puedan proporcionar pistas adicionales

Si después de ambas fases no todos los tipos de parámetros no pueden inferirse, la inferencia falla y deben proporcionarse explícitamente.

#### Unificación de tipos

El proceso de inferencia de tipos resuelve ecuaciones de tipo mediante la unificación de tipos. Este proceso compara recursivamente los dos lados de una ecuación (LHS y RHS), donde uno o ambos tipos pueden ser o contener parámetros de tipo limitantes, y busca los tipos de argumentos correspondientes para hacer que ambos lados de la ecuación sean iguales.

Para este proceso, Go mantiene un mapa que relaciona tipos de parámetros limitantes con sus tipos de argumentos inferidos. Este mapa se actualiza constantemente durante la unificación. Inicialmente, los tipos de parámetros limitantes son conocidos pero sus tipos no, por lo que el mapa está vacío. Durante el proceso, cuando se infiere un nuevo type argument, la relación correspondiente se agrega o actualiza en el mapa.

La unificación utiliza una combinación de unificación exacta y unificación relajada, dependiendo de si ambos tipos deben ser idénticos o solo estructuralmente equivalentes.

Resolver las ecuaciones de tipo es un proceso iterativo. Resolver una ecuación puede llevar a inferir tipos de argumentos que permiten resolver otras ecuaciones. Por esta razón, la inferencia de tipos repite el proceso de unificación de tipos hasta que todos los tipos de argumentos hayan sido inferidos exitosamente.

### Operadores

Los operadores combinan operandos (valores) para formar expresiones.

Para operadores binarios (dos operandos), los tipos de los operandos generalmente deben ser idénticos, con algunas excepciones importantes:
- **Constantes sin tipo:** Si un operando es una constante sin tipo y el otro sí tiene un tipo específico, la constante se convierte al tipo del operando tipado. Esta regla no se aplica a las operaciones de desplazamiento
- **Operaciones de desplazamiento:** En estas operaciones, el operando de lado derecho debe ser un entero o una constante representable por el tipo `uint`. Si el operando de lado izquierdo es una constante sin tipo, se convierte implícitamente al tipo que se asumiría como resultado de la operación de desplazamiento

#### Precedencia de operadores

Los operadores unarios (un operando) tienen la mayor precedencia. Los operadores del mismo nivel de precedencia se asocian de izquierda a derecha.

Existen cinco niveles de precedencia para operadores binarios (dos operandos):

| Nivel | Operador |
|-------|----------|
|   5   | `*`  `/`  `%` `<<` `>>` `&` `&^` |
|   4   | `+` `-` `\|` `^` |
|   3   | `==` `!=` `<` `<=` `>` `>=` |
|   2   | `&&` |
|   1   | `\|\|` |

Los operadores con mayor precedencia se evalúan primero. Los paréntesis pueden usarse para alterar el orden de evaluación por defecto.

### Operadores aritméticos

Los operadores aritméticos se aplican a valores numéricos y producen un resultado del mismo tipo que los operandos. Para la mayoría de operadores binarios (dos valores), ambos operandos deben ser del mismo tipo.

| Operador | Descripción | Tipos |
|----------|-------------|-------|
| `+` | suma | enteros, flotantes, complejos, strings |
| `-` | resta | enteros, flotantes, complejos |
| `*` | multiplicación | enteros, flotantes, complejos |
| `/` | división | enteros, flotantes, complejos |
| `%` | residuo | enteros |
| `&` | AND bitwise | enteros |
| `\|` | OR bitwise | enteros |
| `^` | XOR bitwise | enteros |
| `&^` | bit clear (AND NOT) | enteros |
| `<<` | desplazamiento izquierdo | entero << entero sin signo |
| `>>` | desplazamiento derecho | entero >> entero sin signo |

Si un operando es un tipo de parámetro, el operador debe ser aplicable a todos los tipos en su conjunto de tipos. Los operandos se representan como valores del tipo concreto con el que el tipo de parámetro es instanciado, por lo que la operación se realiza con la precisión de dicho tipo concreto.

#### Operadores de enteros

- **División y módulo:** Para enteros, `/` y `%` están relacionados por la identidad `(a/b)*b + a%b == a` (excepto cuando `b == 0`). La división trunca hacia cero
- **División por cero:** Dividir por cero causa un pánico en tiempo de ejecución
- **Operadores de desplazamiento (`<<`, `>>`):** El operando derecho debe ser sin signo o una constante no negativa. Si es una constante, debe ser menor que el ancho de bits del operando izquierdo

#### Desbordamiento de enteros

- **Enteros sin signo:** Cuando ocurre desbordamiento, se descartan los bits que exceden la capacidad del tipo, implementando un comportamiento de "wrap around" donde el valor regresa al rango válido del tipo
- **Enteros con signo:** El desbordamiento puede ocurrir legalmente, pero el comportamiento específico depende de la implementación del compilador y la arquitectura.

#### Operadores de punto-flotante

- **Operaciones básicas:** `+`, `-`, `*`, `/` siguen el estándar IEEE-754 para números de punto flotante
- **División por cero:** `x/0.0` produce `+Inf` o `-Inf` (no hay pánico)
- **Valores especiales:** Las operaciones pueden producir `+Inf`, `-Inf`, o `NaN` (Not a Number)
- **FMA (Fused Multiply-Add):** Go puede usar instrucciones de hardware que calculan `x*y + z` como una operación atómica con mayor precisión, pero esto depende de la implementación
- **Redondeo:** Sigue las reglas IEEE-754 para redondear al número representable más cercano

#### Concatenación de strings

Los strings se pueden concatenar usando el operador `+` o el operador de asignación `+=`. Estas operaciones siempre crean un nuevo string, ya que los strings en Go son inmutables.

### Operadores de comparación

Los operadores de comparación comparan dos operandos y producen un valor booleano sin tipo.

| Operador | Descripción |
|----------|-------------|
| `==` | igual |
| `!=` | no igual |
| `<` | menor que |
| `<=` | menor o igual que |
| `>` | mayor que |
| `>=` | mayor o igual que |

En cualquier comparasión, el primer operando debe ser asignable al tipo del segundo operando, y vicevesrsa. Los operadores de igualdad (`==` y `!=`) se aplican a operandos comparables, mientras que los operadores de ordenamiento (`<`, `<=`, `>`, `>=`) se aplican a operandos ordenables.

**Tipos comparable y ordenable:**  
- Enteros
- Punto-flotante
- Strings

**Solo comparable:**  
- Booleanos
- Complejos
- Punteros
- Canales

**Comparable condicionalmente:**
- Interfaces (si no son tipos de parámetros)
- Structs (si todos sus campos son comparables)
- Arreglos (si sus elementos son comparables)
- Tipos de parámetro (si son estrictamente comparables)

**Casos especiales:**
- Comparación con `nil`: Los tipos slice, mapa, función, puntero, canal e interfaz pueden compararse con `nil`
- Comparación de interfaces: Si dos valores de tipo interface tienen el mismo tipo dinámico pero ese tipo no es comparable, la comparación produce un pánico en tiempo de ejecución

**Tipos no comparables entre sí:**
- Slices
- Mapas
- Funciones

**Comparaciones entre tipos diferentes:**
- Un valor de tipo no-interfaz puede compararse con un valor de tipo interfaz si el tipo no-interfaz es comparable e implementa la interfaz.

### Operadores lógicos

Los operadores lógicos aplican a valores de tipo booleano y devuelven un valor del mismo tipo que el de los operandos.

| Operador | Descripción |
|----------|-------------|
| `&&` | AND condicional |
| `\|\|` | OR condicional |
| `!` | NOT |

Estos operadores (`&&` y `||`) utilizan *short-circuit evaluation*, esto hace que si un solo lado de la condición provoca que se cumpla o no, el otro lado de la operación ya no se evalúa. Por ejemplo, para `&&` si el lado izquierdo es `false`, el lado derecho no se evalúa y el resultado es `false`; para `||` si el lado izquierdo es `true`, el lado derecho no se evalúa y el resultado es `true`.

Además, cuando sí es necesario evaluar ambos lados de la operación, siempre se evalúa el lado izquierdo y luego el derecho.

### Operadores de dirección

Los operadores de dirección permiten trabajar con punteros y las direcciones de memoria donde se almacenan los valores.

- **Operador de dirección (`&`):** Genera un puntero al operando especificado. El operando debe ser *direccionable*, lo que significa que debe ser una variable, un puntero indirecto, una operación de indexado de slice, un campo de struct direccionable, o una operación de indexado de un arreglo direccionable
- **Operador de indirección (`*`):** Realiza la desreferenciación de un puntero para obtener el valor almacenado en la dirección de memoria a la que apunta. Si se aplica a un puntero `nil`, la operación causa un pánico en tiempo de ejecución
- **Direcionalidad:** No todos los valores son direccionables. Por ejemplo, las literales, constantes, y los resultados de la mayoría de expresiones no son direccionables. Solo se puede obtener la dirección de valores que tienen una ubicación específica en memoria
- **Relación entre operadores:** Estos operadores son inversos entre sí. Si `x` es *direccionable*, entonces `*(&x)` es equivalente a `x`. Si `p` es un puntero válido, entonces `&(*p)` es equivalente a `p`.

### Operador de recepción

El operador de recepción `<-` es específico para los canales, y permite recibir un valor de un canal `canal`. El canal debe permitir operaciones de recepción, y el tipo del resultado es el tipo de elemento del canal. Esta expresión bloquea la rutina go actual hasta que un valor esté disponible en el canal. Recibir de un canal `nil` bloquea indefinidamente.

Es posible recibir de un canal cerrado. En este caso, la operación retorna inmediatamente el valor cero del tipo de elemento del canal si dicho canal está vacío. La expresión de recepción puede usarse en una asignación de dos valores: `valor, ok := <-canal`. El segundo valor es un booleano sin tipo que indica si la recepción fue exitosa, `ok` es `true` si el valor fue enviado por una operación de envío exitosa, y `false` si es un valor cero porque el canal está cerrado y vacío.

Si el operando es un tipo de parámetro, todos los tipos en su conjunto de tipos deben ser tipos canal que permitan operaciones de recepción y tengan el mismo tipo de elemento.

### Conversiones

Una conversión cambia el tipo de una expresión al tipo especificado. Las conversiones pueden aparecer directamente en la expresión (explícitas) o estar implícitas por el contexto en el que aparece la expresión.

La conversión explícita tiene la forma `T(x)` donde `T` es el tipo y `x` es una expresión que puede ser convertida a dicho tipo. Si la expresión inicia con algún operador especial (`*`, `<-`) es necesario encerrar el operador y su operando entre paréntesis para evitar ambigüedades.

Un valor constante puede ser convertido a un tipo si dicho valor puede ser representado por el tipo. Convertir una constante que no es un tipo de parámetro genera una constante tipada. Por el otro lado, convertir una constante que es un tipo de parámetro genera un valor no constante de dicho tipo representado por el tipo con el que fue instanciado el tipo de parámetro.

Reglas para la conversión de un valor no constante:
* `x` es asignable a `T`
* `x` y `T` no son tipos de parámetro pero su tipo subyacente es idéntico
* `x` y `T` son tipo puntero, no son tipos nombrados y sus tipos base son idénticos
* `x` y `T` son de tipo entero o punto flotante
* `x` y `T` son de tipo complejo
* `x` es de tipo entero o slice de bytes o runes y `T` es de tipo string
* `x` es de tipo string y `T` de tipo slice de bytes o runes
* `x` es de tipo slice, `T` es de tipo arreglo o puntero a un arreglo y el tipo de sus elementos es idéntico

Las conversiones específicas que aplican a valores no constantes de tipos numéricos o de tipo string pueden cambiar la representación de dicha variable y representar un costo extra en la ejecución. Todas las otras conversiones solo cambian el tipo pero no la representación de la variable.

#### Conversiones entre tipos numéricos

Para conversiones de valores numéricos no constantes, se aplican las siguientes reglas:
1. Al convertir entre tipos enteros, si el valor es un entero con signo, se extiende el signo; de lo contrario, se extiende con ceros. Por lo tanto, la conversión siempre genera un valor válido sin indicación de desbordamiento
2. Al convertir punto-flotante a entero, la parte fraccionaria es descartada truncando hacia cero
3. Al convertir entero o punto-flotante a punto-flotante, o de complejo a otro tipo complejo, el resultado es redondeado a la precisión del tipo destino

En todas las conversiones no-constantes que involucren valores de tipo punto-flotante o complejo, si el tipo del resultado no puede representar el valor, la conversión es exitosa pero el resultado dependerá de la implementación.

#### Conversiones de y hacia tipos string

1. Convertir un slice de bytes a un string genera un string cuyos bytes consecutivos son los elementos del slice
2. Convertir un slice de runes a un string genera un string que es la concatenación de los valores rune individuales convertidos a string
3. Convertir un string a slice de bytes genera un slice no-nil cuyos elementos consecutivos son los bytes utilizados para representar el string
4. Convertir un string a slice de runes genera un slice que contiene los code-points Unicode individuales del string
5. Por razones históricas, un integer puede ser convertido a string, generando un string que contiene la representación en UTF-8 del code-point Unicode correspondiente al integer. Es decir, el integer es tratado como un code-point Unicode

#### Conversiones de slice a arreglo

Convertir un slice a un arreglo genera un arreglo que contiene los elementos del arreglo subyacente del slice. De forma similar, convertir un slice a un puntero a un arreglo genera un puntero al arrerglo subyacente del slice. En ambos casos, si la longitud del slice es mayor a la longitud del arreglo, ocurre un pánico en tiempo de ejecución.

### Expresiones constantes

Las expresiones constantes solo pueden contener operandos constantes y son evaluadas en tiempo de compilación.

Constantes booleanas, numéricas, y strings sin tipo pueden ser usadas como operandos donde sea permitido el uso de dichos tipos respectivamente.

Una comparación de constantes siempre genera una constante booleana sin tipo. Si el operando izquierdo en una expresión de desplazamiento es una constante sin tipo, el resultado es una constante entera; de lo contrario, es una constante del mismo tipo que el operando izquierdo, el cual debe ser de tipo entero.

Cualquier operación en constantes sin tipo resulta en una constante sin tipo que tiene la misma categoría. En operaciones binarias (dos operandos) con operandos sin tipo de diferentes categorías, el resultado toma la categoría del operando que aparece más tarde en esta lista siguiendo una jerarquía: entero, rune, punto-flotante, complejo. Esto es con el objetivo de contener ambos operandos mantiendo una pérdida conceptual mínima.

Las expresiones constantes siempre son evaluadas de forma exacta. Los valores intermedios y las propias constantes pueden requerir precisión significativamente mayor que cualquier tipo predefinido. Por lo tanto, las constantes mantienen una mayor precisión de representación que cualquier otro tipo predefinido en Go. Sin embargo, los valores de constantes siempre deben ser representables exactamente por el tipo al que se convierten.

### Orden de evaluación

A nivel de paquete, las dependencias de inicialización (entre variables) determinan el orden de evaluación de las expresiones individuales de inicialización en declaraciones de variables. Sin embargo, al evaluar los operandos de una expresión, asignación o declaración de retorno, todos los operandos (llamadas a funciones, llamadas a métodos, operaciones de recepción de canales, y operaciones lógicas binarias) son evaluados en orden léxico de izquierda-a-derecha.

Por lo tanto, dichas dependencias de inicialización pueden anular la regla de evaluación de izquierda-a-derecha para las inicializaciones a nivel de paquete, pero no pueden cambiar el orden de evaluación de los operandos dentro de cualquier expresión individual.

## Sentencias

Las sentencias son instrucciones completas que controlan la ejecución y son la forma más general del lenguaje, es decir, que las sentencias engloban prácticamente todos los demás elementos más específicos del lenguaje (expresiones, declaraciones, etc.).

### Sentencias de terminación

Una sentencia de terminación interrumpe el flujo de control regular dentro de un bloque. Es decir, que este tipo de sentencias no solo finalizan la ejecución de un bloque, sino que también controlan el flujo de ejecución, modificando el flujo procedimental en el que se presenta el código del bloque.

Las siguientes son las sentencias de terminación en Go:
1. La sentencia `return` o `goto`
2. Llamar a la función integrada `panic()`
3. Un bloque en que su lista de sentencias termina con una sentencia de terminación
4. La sentencia `if` en la que:
    - la rama del `else` está presente
    - ambas ramas (`if` y `else`) terminan con sentencias de terminación
5. La sentencia `for` en la que:
    - no hay sentencias `break` correspondientes al bucle 
    - no hay condición del bucle
    - no se usa la palabra reservada `range`
6. La sentencia `switch` en la que:
    - no hay sentencias `break` correspondientes a la estructura
    - hay un caso `default`
    - todos los casos, incluyendo el `default`, terminan con una sentencia de terminación
7. La sentencia `select` en la que:
    - no hay sentencias `break` correspondientes a la estructura
    - hay un caso `default`
    - todos los casos, incluyendo el `default`, terminan con una sentencia de terminación
8. Las sentencias de etiqueta que terminan con una sentencia de terminación

Todas las otras sentencias no son de terminación, por lo que no interrumpen ni modifican el flujo de control del bloque en que se encuentran. Una lista de sentencias termina con una sentencia de terminación si: la lista no está vacía, y su sentencia final es una sentencia de terminación.

### Sentencias vacías

Las sentencias vacías no hacen nada y consisten únicamente en un punto y coma.

### Sentencias etiquetadas

Las sentencias etiquetadas pueden ser los destinos de las sentencias `goto`, `break` o `continue`. Estas siguen la estructura: `Etiqueta:Sentencia`.

### Sentencias expresivas

Excepto las funciones integradas en el lenguaje, las llamadas a funciones y métodos, y las operaciones de recepción de canales (`<-`) pueden ser usadas como sentencias.

### Sentencias de envío

Este tipo de sentencias son aquellas usadas para enviar valores a un canal.

Para que estas sentencias sean válidas deben ser usadas en un canal que permita envío y el tipo del valor a enviar debe ser asignable al tipo del elemento del canal. Tanto la expresión del canal como el valor a enviar son evaluadas antes de que ocurra la comunicación.

En el caso de canales sin buffer, se bloquea la ejecución hasta que ambos lados de la comunicación estén listos. Por lo tanto, enviar en un canal sin buffer ocurre si el valor será recibido; enviar en un canal con buffer ocurre si hay espacio en el buffer. Sin embargo, enviar a un canal cerrado causa un pánico en tiempo de ejecución; y enviar a un canal `nil` bloquea indefinidamente.

Además, si el tipo del canal es un tipo de parámetro, su conjunto de tipos debe contener solo tipos canal con la misma direccionalidad.

### Sentencias de incremento/decremento

Las sentencias de incremento `++` y decremento `--` sirven para incrementar o decrementar su operando en uno, respectivamente.

Para poder ser usadas, su operando debe ser un elemento del cual se pueda obtener su dirección y los operadores deben aparecer después del operando.

### Sentencias de asignación

Una asignación reemplaza el valor actual almacenado en una variable con un nuevo valor especificado por una expresión. Este tipo de sentencias puede asignar un único valor a una única variable o múltiples valores a múltiples variables.

El lado izquierdo de cualquier operación de asignación debe ser un operando direccionable, o ser el identificador en blanco (`_`). Los operandos del lado izquierdo pueden estar entre paréntesis.

Una operación de asignación compuesta con la forma  `x op= y` y donde `op` es un operador binario, es equivalente a la forma `x = x op (y)` pero `x` se evalúa solo una vez. La parte `op=` es un único token. En este tipo de operaciones, tanto el lado izquierdo como el lado derecho deben contener exactamente una expresión que produzca un único valor, y el lado izquierdo no debe ser el identificador en blanco.

Una asignación múltiple asigna los elementos individuales de una operación de múltiples valores a una lista de variables. Existen dos formas: la primera, la parte derecha de la operación es una expresión de múltiples valores como una función con varios valores de retorno; la segunda, el número de operandos en ambos lados es igual y cada valor forma un par con su variable correspondiente.

El identificador en blanco (`_`) proporciona una forma de ignorar valores en una sentencia de asignación.

La asignación ocurre en dos fases: primero, los operandos del lado izquierdo y las expresiones del lado derecho son evaluadas en el orden usual; segundo, las asignaciones se realizan de izquierda a derecha.

Todos los valores deben ser asignables a las variables correspondientes, excepto en los siguientes casos:
- Cualquier valor puede ser asignado al identificador en blanco
- Si una constante sin tipo es asignada a una variable de tipo interfaz o al identificador en blanco, dicha constante primero es convertida a su tipo predeterminado
- Si una constante booleana sin tipo es asignada a una variable de tipo interfaz o al identificador en blanco, primero es convertida al tipo `bool`

Cuando un valor es asignado a una variable, solo el contenido almacenado en dicha variable es reemplazado. Si el valor contiene una referencia, la asignación copia la referencia pero no crea una copia de los datos referenciados.

### Sentencias if

Las sentencias `if` especifican la ejecución condicional de dos ramas dependiendo del valor de una expresión booleana. Si la expresión se evalúa como `true`, se ejecuta la rama `if`; de lo contrario, si la rama `else` se encuentra presente, se ejecuta dicha rama.

La expresión puede ser precedida por una sentencia de asignación simple, la cual se ejecuta antes de que la expresión de la condición sea evaluada.

### Sentencias switch

Las sentencias `switch` proporcionan ejecución de múltiples ramas, donde una expresión o tipo es comparado con cada uno de los `case` dentro de la sentencia para determinar qué rama ejecutar.

Hay dos formas: **switch de expresión** y **switch de tipo**. En la primera, los casos contienen expresiones que son comparadas con la expresión del `switch`; en la segunda, los casos contienen tipos que son comparados con el tipo de la expresión del `switch`.

#### Switch de expresión

En un switch de expresión, la expresión es evaluada primero; luego, las expresiones de cada caso, que no necesitan ser constantes, son evaluadas de izquierda-a-derecha y de arriba-hacia-abajo. El primer caso cuya expresión sea igual a la expresión del switch será ejecutado y todos los otros casos son ignorados. Si ningún caso coincide, se ejecutará el caso `default`, si está presente, y puede estar en cualquier lugar del switch. Una expresión de switch ausente es tomada como el valor booleano `true`.

Si la expresión del switch evalúa a una constante sin tipo, primero se convierte a su tipo predeterminado. El valor `nil` no puede ser usado como expresión del switch. El tipo de la expresión del switch debe ser comparable.

La expresión del switch es tratada como si fuera el operando derecho de una comparación con cada expresión de case, y la expresión del switch puede ir precedida de una sentencia de asignación simple, la cual es ejecutada antes de que la expresión sea evaluada.

#### Switch de tipo

En un switch de tipo se comparan tipos en lugar de valores. Es similar a un switch de expresión, pero utiliza una expresión con una forma de aserción de tipo (`x.(tipo)`) usando la palabra reservada `type` en lugar de un tipo específico.

Al igual que con las aserciones de tipo, `x` debe ser de tipo interfaz para poder obtener su tipo dinámico. Los cases contienen tipos y deben ser únicos.

En estos switches, al menos un caso puede usar el valor `nil`. También, tipos de parámetro pueden ser usados en los casos; en este caso, se usa el tipo de la instanciación, y si un tipo se repite, se selecciona el primer case que coincida.

### Sentencias for

Las sentencias `for` especifican la ejecución repetitiva de un bloque. Existen tres formas de controlar las iteraciones: usando únicamente una condición, usando la forma completa del `for` o usando `range`.

#### Sentencias for con una única condición

Esta es la forma más simple de la sentencia; la condición se evalúa antes de cada iteración y si evalúa a `true` se ejecutará la iteración; de lo contrario, el bucle finalizará. Si la condición está ausente, siempre se evaluará como `true`, lo que crearía un bucle infinito.
- Ejemplo:
    ```Go
    for a < b {
        a = b * 2
    }
    ```

#### Sentencias for completas

Esta es la forma completa de la sentencia, también es controlada por una condición, pero adicionalmente puede especificar una sentencia inicial que se ejecuta antes de la primera iteración, y una sentencia post que se ejecuta después de cada iteración. La sentencia inicial puede ser una declaración corta de una variable. Las tres partes (inicial, condición, post) deben estar separadas por `;`.
- Ejemplo:
    ```Go
    for i := 0; i < 10; i++ {
        funcion(i)
    }
    ```

La sentencia inicial se ejecuta antes de evaluar la condición para la primera iteración, y la sentencia post se ejecuta después de que una iteración se haya completado. Cualquier elemento puede estar vacío, pero los `;` deben estar presentes.

Cada iteración tiene sus propias variables declaradas. La variable de la primera iteración es declarada por la sentencia inicial. Las variables para las iteraciones siguientes son declaradas implícitamente antes de ejecutar la sentencia post y son inicializadas con el valor de la iteración anterior en ese momento.

#### Sentencias for usando range

La sentencia `for` junto con la cláusula `range` itera sobre todos los elementos de un arreglo, slice, string, mapa, valores recibidos de un canal, valores enteros, o valores de una función que genera iteradores.
- Ejemplo:
    ```Go
    for indice, valor := range arreglo {
        arreglo[indice] = valor * 2
    }
    ```

La expresión a la derecha correspondiente a la cláusula range es llamada **expresión range**, la cual puede ser un arreglo, puntero a un arreglo, slice, string, mapa, canal, entero, o una función con cierta firma. Al igual que con las asignaciones, los operandos del lado izquierdo deben ser direccionables y representan las variables de iteración. Si la expresión range es una función, el número máximo de variables de iteración depende de la firma de la función. Si la range expression es un channel o entero, se permite máximo una variable de iteración.

La expresión range es evaluada una vez antes de comenzar el bucle, con una excepción: si hay solo una variable de iteración y tanto la expresión range como su longitud son constantes, entonces la evaluación puede optimizarse.

Las variables de iteración pueden ser declaradas usando declaración corta y pertenecen únicamente al scope del bloque `for`, manteniendo un valor único para cada iteración. Su tipo depende de los tipos correspondientes de la expresión range. Si no se usa esta forma, las variables deben haber sido declaradas anteriormente.

Si la expresión range es un tipo de parámetro, todo su conjunto de tipos debe contener tipos del mismo tipo de datos compatibles con la cláusula range.

### Sentencias go

La sentencia `go` inicia la ejecución de una llamada a una función de forma concurrente dentro del mismo espacio de memoria. A esto se le conoce como **rutinas go (goroutines)**.
- Ejemplo:
    ```Go
    go function(args)
    ```

La expresión debe ser una llamada a una función o a un método y no puede estar entre paréntesis. Las llamadas a funciones integradas están restringidas a sentencias de expresiones únicamente.

La función y sus argumentos son evaluados inmediatamente en la rutina go actual, pero, a diferencia de una llamada regular, el programa no espera a que la función actual termine para continuar su ejecución. El planificador de Go gestiona cuándo iniciar la ejecución de la nueva rutina go. Cuando la función puesta en una nuevo rutina go termina de ejecutarse, la rutina go en la que se puso también finaliza, y si la función tiene valores de retorno, estos son descartados.

### Sentencias select

La sentencia `select` elige un caso de un conjunto, cuyas expresiones son operaciones de envío o recepción usando canales. Esto es similar a un `switch` con la diferencia de que el caso que se elige es el que esté listo primero.

Esta sentencia permite trabajar con operaciones de canales basándose en la operación que pueda ser realizada, evitando bloqueos de la rutina go actual. También, puede haber un caso `default`, que será elegido en caso de que ninguna operación de canal pueda ser realizada en ese momento.

La ejecución de un select sucede en varios pasos:
1. **Evaluación:** Para todos los casos en la sentencia, las expresiones de canal y los valores a enviar son evaluadas una vez, en el orden en que aparecen. El resultado es un conjunto de canales para recibir o enviar valores y sus valores correspondientes. Los efectos-secundarios de estas evaluaciones ocurren inmediatamente. Las variables del lado izquierdo (para recepción) aún no son evaluadas en este paso
2. **Selección:** Si varias operaciones pueden proceder, Go elige solo una de forma pseudoaleatoria. Si ninguna puede proceder, se elige el caso default si está presente; si no está presente, la ejecución se bloquea hasta que alguna operación pueda proceder
3. **Comunicación:** A menos que el caso default haya sido seleccionado, la operación de comunicación seleccionada se ejecuta
4. **Asignación:** Si hay variables en el lado izquierdo, se les asigna el valor resultante de la operación de comunicación
5. **Ejecución:** El código del caso seleccionado es ejecutado

Debido a que las operaciones en canales `nil` bloquean indefinidamente, un `select` con solo canales `nil` y sin caso default se bloquea indefinidamente.

### Sentencias return

La sentencia `return` solo puede ser usada dentro de una función, y esta finaliza la ejecución de la función donde sea usada, opcionalmente puede proveer uno o más resultados al lugar de la llamada a dicha función.

Es importante mencionar que las funciones `defer` se ejecutan justo antes de que la función termine, ya sea por una sentencia `return` o al llegar al final de la función.

Es posible usar `return` en una función que no devuelve ningún valor, pero la sentencia no debe especificar ningún valor de retorno, por lo que se usa únicamente para terminar la ejecución de la función anticipadamente.

Hay tres formas de retornar valores desde una función:
1. Los valores de retorno son explícitamente listados en la sentencia return, donde cada valor debe ser asignable al tipo de elemento correspondiente definido en la firma de la función
2. La expresión en la lista de la sentencia return puede ser una llamada a otra función que retorne valores que coincidan con los tipos definidos en la firma de la función
3. La lista de return puede estar vacía (*bare return*) cuando los parámetros de retorno están nombrados en la firma de la función. En este caso, se retornan automáticamente los valores actuales de esas variables nombradas

Independientemente de cómo sean declarados los valores a retornar, todos son inicializados con sus valores cero correspondientes inmediatamente después de entrar a la función. Una sentencia return que especifica valores explícitos asigna esos valores a los parámetros de retorno antes de ejecutar cualquier función defer.

### Sentencias break

La sentencia `break` finaliza la ejecución de la sentencia `for`, `switch` o `select` más interna dentro de la misma función.

Opcionalmente, `break` puede incluir una etiqueta que corresponda a una sentencia `for`, `switch` o `select` específica. En este caso, la ejecución terminará en esa sentencia etiquetada en lugar de la más interna.

### Sentencias continue

La sentencia `continue` finaliza la iteración actual y pasa a la siguiente iteración de la sentencia `for` más interna. Esto lo hace al transferir el control de flujo al final del bloque del bucle, donde se evalúa la condición de continuación y se ejecuta la sentencia post (si existe).

De igual forma que la sentencia `break`, puede incluir una etiqueta que corresponda a una sentencia for específica. En este caso, será ese bucle etiquetado el que pase a su siguiente iteración, no necesariamente el más interno.

### Sentencias goto

La sentencia `goto` transfiere el control de flujo al punto donde se encuentra la etiqueta especificada, pero esto solo es posible dentro de la misma función.

Es importante entender que la ejecución de `goto` no debe causar que se omita la declaración de alguna variable que esté en el alcance de la etiqueta de destino. En otras palabras, no se puede usar `goto` para saltar la declaración de una variable si esa variable sería visible en el punto de destino.

Además, `goto` no puede transferir control a una etiqueta que esté dentro de un bloque al cual la sentencia `goto` no tiene acceso desde su posición actual.

### Sentencias fallthrough

La sentencia `fallthrough` transfiere el control de flujo al primer caso inmediatamente siguiente dentro de una sentencia de un **switch de expresión**. Solo puede ser usada como la última sentencia en un caso no vacío de un `switch`.

Esta sentencia existe porque Go, a diferencia de lenguajes como C o Java, no tiene *fallthrough* automático en las sentencias switch. En Go, cada caso termina automáticamente después de ejecutarse, por lo que *fallthrough* debe usarse explícitamente cuando se desea continuar al siguiente caso.

Es importante notar que *fallthrough* no evalúa la condición del siguiente caso, simplemente ejecuta las sentencias del case siguiente incondicionalmente.

### Sentencias defer

La sentencia `defer` programa la ejecución de una función para que sea invocada únicamente cuando la función que la contiene está a punto de terminar. Esto puede ocurrir cuando la función completa normalmente su ejecución, ejecuta una sentencia `return`, o cuando la rutina go correspondiente entra en pánico.

La expresión debe ser únicamente una llamada a función o método, y no puede estar entre paréntesis. El uso de funciones integradas está restringido únicamente a `copy`, `delete`, `print`, `println` y `recover`.

Cuando se ejecuta la sentencia `defer`, los argumentos de la función son evaluados inmediatamente, pero la función en sí no es invocada hasta que la función contenedora termine. Las funciones defer se ejecutan en orden LIFO (Last In, First Out), es decir, en orden inverso al que fueron declaradas.

Es crucial entender que las funciones `defer` se ejecutan después de que la sentencia `return` haya asignado valores a los parámetros de retorno, pero antes de que la función termine completamente y retorne al lugar de la llamada. Esto permite que las funciones `defer` puedan leer y modificar los valores de retorno nombrados.

Si la función especificada en defer evalúa a `nil`, ocurre un pánico cuando dicha función es invocada, no cuando se evalúa la sentencia defer.

## Funciones integradas

Todas las funciones integradas en el lenguaje son predeclaradas. Dichas funciones no tienen un tipo estándar, por lo que solo pueden aparecer en expresiones de llamada y no pueden ser asignadas a variables o pasadas como valores a otras funciones. Se invocan como cualquier otra función, pero algunas de ellas pueden aceptar diferentes tipos como argumentos.

### Añadir a y copiar slices

Las funciones integradas `append` y `copy` permiten operaciones comunes en slices. El resultado de ambas funciones es independiente de si comparten el mismo espacio de memoria subyacente con los argumentos.

La función variádica `append` agrega cero o más valores a un slice y devuelve el slice resultante del mismo tipo. Los valores adicionales son pasados al parámetro de tipo `...E`, donde `E` es el tipo de elemento del slice. Si la capacidad del slice no es suficiente para almacenar los nuevos elementos, `append` asigna un nuevo arreglo subyacente con capacidad suficiente (generalmente el doble de la capacidad anterior) y copia todos los elementos existentes junto con los nuevos.

La función `copy` copia elementos de un slice fuente a un slice destino y devuelve el número de elementos efectivamente copiados. Ambos slices deben tener tipos de elementos idénticos. La cantidad de elementos copiados corresponde al mínimo entre las longitudes de ambos slices.

Para ambas funciones, cuando se usan con tipos de parámetro genéricos, todos los tipos en su conjunto de tipos deben tener el mismo tipo subyacente.

### Clear

La función integrada `clear` toma como argumento un mapa, slice o tipo de parámetro, y elimina todos sus elementos o los regresa a su valor cero.

Para mapas, `clear` elimina todas las entradas, dejando el mapa vacío pero utilizando el mismo espacio de memoria subyacente. Para slices, `clear` establece todos los elementos a su valor cero, pero mantiene la longitud original del slice.

Si el argumento es un tipo de parámetro, todo su conjunto de tipos debe consistir únicamente de tipos mapa o slice, para que la función pueda operar independientemente del tipo concreto con el que se instancie el tipo de parámetro.

Si el argumento es `nil`, la función no realiza ninguna operación (no-op).


### Close

La función integrada `close` sirve únicamente para canales, e indica que no se enviarán más valores a través de dicho canal. El canal debe permitir operaciones de envío (no puede ser un canal de solo recepción).

Enviar valores a un canal cerrado, intentar cerrar un canal ya cerrado, o cerrar un canal `nil` provoca un pánico en tiempo de ejecución. Una vez que un canal ha sido cerrado y todos sus valores pendientes han sido recibidos, las operaciones de recepción del canal retornarán el valor cero del tipo de elemento del canal sin bloquear las rutinas go.

Si el argumento es un tipo de parámetro, todo su conjunto de tipos debe consistir únicamente de tipos canal con la direccionalidad correcta (que permita envío), para que la función pueda operar independientemente del tipo concreto con el que se instancie el tipo de parámetro.

### Manipulación de números complejos

Existen tres funciones integradas para trabajar con números complejos. La función `complex` construye un número complejo utilizando una parte real y una parte imaginaria de punto flotante; las funciones `real` e `imag` extraen respectivamente la parte real e imaginaria de un número complejo.

Para `complex`, ambos argumentos deben ser del mismo tipo de punto flotante y el valor retornado corresponde al tipo complejo asociado: `complex64` para argumentos `float32`, o `complex128` para argumentos `float64`. Si uno de los argumentos es una constante sin tipo, se convierte implícitamente al tipo del otro argumento. Si ambos argumentos son constantes sin tipo, no deben ser números complejos y la parte imaginaria debe ser cero, en este caso, el valor retornado es una constante compleja sin tipo.

Para `real` e `imag`, el argumento debe ser de tipo complejo y el valor retornado es del tipo de punto flotante correspondiente: `float32` para `complex64`, o `float64` para `complex128`. Si el argumento es una constante sin tipo, el valor retornado es una constante de punto flotante sin tipo.

Estas funciones no admiten argumentos de tipo de parámetro.

### Elemininación de elementos de un mapa

La función integrada `delete` elimina el elemento correspondiente a la clave especificada dentro de un `map`. La clave debe ser asignable al tipo de clave definido para el mapa.

Si el primer argumento es un tipo de parámetro, su conjunto de tipos debe contener únicamente tipos mapa, y todos esos tipos mapa deben tener el mismo tipo de clave.

Si el mapa es `nil` o la clave no existe en el mapa, la función no realiza ninguna operación (no-op).

### Longitud y capacidad

Las funciones integradas `len` y `cap` aceptan argumentos de diferentes tipos y siempre devuelven un resultado de tipo `int`.

Si el argumento es un tipo de parámetro, el uso de la función correspondiente debe ser válido para todos los tipos en su conjunto de tipos, y el resultado corresponde a la longitud o capacidad del valor del tipo concreto utilizado al instanciar dicho tipo de parámetro.

La longitud y capacidad tienen significados específicos según el tipo:
**Longitud (`len`):**  
- **String:** número de bytes en la representación UTF-8 del string
- **Arreglo:** número de elementos en el arreglo (fijo en tiempo de compilación)
- **Slice:** número de elementos actualmente en el slice
- **Mapa:** número de pares clave-valor definidos
- **Canal:** número de elementos actualmente en el buffer del canal

**Capacidad (`cap`):**
- **Arreglo:** número de elementos en el arreglo (igual que `len` para arreglos)
- **slice:** número máximo de elementos que puede contener el arreglo subyacente desde la posición actual
- **Canal:** capacidad máxima del buffer del canal

Cuando los argumentos son constantes evaluables en tiempo de compilación, el resultado también es una constante y puede ser optimizado por el compilador.

### Crear mapas, slices y canales

La función integrada `make` toma un tipo de slice, mapa, canal o tipo de parámetro, opcionalmente seguido por argumentos que especifican propiedades del objeto a crear. Esta función retorna un valor completamente inicializado del tipo especificado, donde la memoria subyacente es inicializada apropiadamente (valores cero).

**Slice:**  
- `make([]T, n)`: slice de tipo `[]T` con longitud `n` y capacidad `n`
- `make([]T, n, m)`: slice de tipo `[]T` con longitud `n` y capacidad `m`

**Mapa:**  
- `make(map[K]V)`: mapa vacío de tipo `map[K]V`
- `make(map[K]V, n)`: mapa de tipo `map[K]V` con espacio pre-asignado para aproximadamente `n` elementos

**Canal:**  
- `make(chan T)`: canal sin buffer de tipo chan `T` (síncrono)
- `make(chan T, n)`: canal de tipo chan `T` con buffer de capacidad `n`

**Tipo de parámetro:** todo su conjunto de tipos debe contener únicamente tipos slice, mapa o canal que compartan el mismo tipo subyacente. Para canales, todos deben tener la misma direccionalidad.

Los argumentos de tamaño (`n` y `m`) deben ser expresiones enteras no negativas representables como tipo `int`. Para slices, `n` no debe ser mayor que `m`.

### Mínimo y máximo

Las funciones integradas `min` y `max` devuelven respectivamente el valor mínimo y máximo de un conjunto fijo de argumentos de tipos ordenables. Debe proporcionarse al menos un argumento.

Para que los argumentos sean válidos, deben cumplir las mismas reglas que los operadores de comparación: todos los argumentos deben ser comparables entre sí, similar a como `x + y` debe ser válido para argumentos numéricos. Si todos los argumentos son constantes, el resultado también es una constante.

Para argumentos numéricos enteros, estas funciones son conmutativas y asociativas, por lo que el orden de los argumentos no afecta el resultado.

Para argumentos de punto flotante, existen reglas especiales para manejar casos como cero negativo (-0), NaN (Not a Number), e infinito, siguiendo el estándar IEEE 754. Estas reglas son intuitivas: NaN se propaga (si algún argumento es NaN, el resultado es NaN), y se respetan las comparaciones estándar para infinitos y ceros con signo.

Para argumentos de tipo string, la comparación se realiza lexicográficamente byte por byte.

Si el argumento es un tipo de parámetro, todos los tipos en su conjunto de tipos deben ser ordenables y comparables entre sí.

### Asignación de memoria

La función integrada `new` recibe como argumento un tipo y asigna memoria para un valor de ese tipo. Esta función retorna un puntero a la memoria asignada, donde el valor está inicializado con su valor cero correspondiente.

Es importante notar que `new` funciona con cualquier tipo, y siempre retorna un puntero al tipo especificado. Por ejemplo, `new(int)` retorna `*int`.

La ubicación específica de la memoria (heap vs stack) es un detalle de implementación que el tiempo de ejecución de Go decide mediante *escape analysis* (técnica para saber si el alcance de una variable va más allá del alcance donde se declaró), no algo que el programador controla directamente.

### Gestionar pánicos

Las funciones integradas `panic` y `recover` brindan asistencia para reportar y gestionar errores en tiempo de ejecución y condiciones excepcionales del programa.

Cuando se ejecuta una función y ocurre una llamada explícita a `panic` o surge un error en tiempo de ejecución, la ejecución normal de esa función se detiene inmediatamente. Sin embargo, cualquier función `defer` previamente registrada se ejecuta normalmente. Este proceso continúa subiendo por la pila de llamadas: cada función en la cadena se detiene, pero sus `defer`s se ejecutan. Si ninguna función `defer` llama a `recover`, el programa eventualmente termina y reporta el error. Esta secuencia se conoce como *panicking*.

La función `recover` permite a un programa interceptar y manejar el comportamiento de una rutina go en pánico. Además, `recover` retorna el valor que fue pasado a `panic` cuando:
- La rutina go está en estado de pánico
- `recover` es llamada directamente desde una función `defer`

En cualquier otro caso (rutina go no está en pánico, o recover no es llamada desde defer), `recover` retorna `nil` y no tiene efecto.

Es importante notar que llamar a `panic` con valor `nil` sí causa un pánico en tiempo de ejecucicón, pero `recover` puede detectarlo y retornará `nil` como valor recuperado.

### Arranque

Go provee algunas funciones integradas que son útiles durante el arranque o inicialización de un programa (bootstrapping). Aunque están documentadas para completitud, estas funciones no tienen garantía de compatibilidad y pueden cambiar o eliminarse en versiones futuras del lenguaje.

Estas funciones no retornan ningún valor y están pensadas principalmente para depuración a bajo nivel o situaciones donde las facilidades normales de E/S no están disponibles:
- `print`: imprime todos sus argumentos directamente a la salida estándar, concatenados sin separadores
- `println`: imprime todos sus argumentos separados por espacios, con una nueva línea al final

Es importante entender que estas funciones operan a un nivel más bajo que `fmt.Print` y `fmt.Println`, y su comportamiento específico puede depender de la implementación del tiempo de ejecución.

## Paquetes

Los programas de Go se construyen enlazando varios paquetes que trabajan en conjunto para formar un programa ejecutable. Un paquete se construye a partir de uno o más archivos de código fuente que juntos declaran constantes, variables, tipos, funciones y otros elementos de Go. Estos elementos son accesibles en todos los archivos del mismo paquete, y pueden ser accesibles desde otros paquetes si son exportados (comienzan con mayúscula).

### Optimización de archivos fuente

Cada archivo fuente debe contener:
- **Palabra reservada `package`:** define a qué paquete pertenece el archivo
- **Declaraciones de importación:** conjunto posiblemente vacío de declaraciones que especifican qué paquetes usar
- **Declaraciones de alto-nivel :** conjunto posiblemente vacío de declaraciones de constantes, variables, tipos, funciones, etc.

### Package

La cláusula `package` debe aparecer al inicio de cada archivo fuente y define a qué paquete pertenece dicho archivo. El nombre del paquete no puede ser el identificador en blanco (`_`).

Un conjunto de archivos que comparten el mismo nombre de paquete forman la implementación de ese paquete. Típicamente, todos los archivos de un paquete deben residir en el mismo directorio, aunque esto puede depender de la implementación del sistema de compilación.

### Declaraciones de importación

Una declaración `import` establece que el archivo contenedor depende de la funcionalidad del paquete importado, permitiendo el acceso a los identificadores exportados de dicho paquete. Cada declaración `import` especifica un identificador local (nombre del paquete) y una ruta de importación (ubicación del paquete).

El identificador local se usa como identificador calificado para acceder a elementos exportados del paquete importado. Si el identificador se omite, se usa por defecto el nombre declarado en la cláusula `package` del paquete importado. Si se usa el identificador `.`, todos los identificadores exportados del paquete se importan al alcance actual, eliminando la necesidad de identificadores calificados.

La interpretación de la ruta de importación depende de la implementación, pero típicamente representa una ruta que identifica únicamente al paquete, a menudo relacionada con repositorios de control de versiones.

Una declaración `import` establece una dependencia del paquete importador hacia el importado. No está permitido que un paquete se importe directa o indirectamente a sí mismo (dependencias circulares). Para importar un paquete únicamente por sus efectos secundarios de inicialización, se puede usar el identificador en blanco `_`.

## Inicialización y ejecución de un programa

### El valor cero

Cuando se asigna memoria para una variable, ya sea mediante una declaración, el uso de `new`, literales compuestas o `make`, y no se proporciona inicialización explícita, la variable recibe automáticamente su valor cero (zero value).

Cada tipo tiene su propio valor cero específico:
- Booleanos: `false`
- Tipos numéricos enteros: `0`
- Tipos numéricos de punto flotante: `0.0`
- Tipos numéricos complejos: `0+0i`
- Strings: `""` (string vacío)
- Punteros: `nil`
- Funciones: `nil`
- Interfaces: `nil`
- Slices: `nil`
- Canales: `nil`
- Mapas: `nil`

Esta inicialización se aplica recursivamente, por ejemplo, cada elemento de un arreglo, cada campo de un struct, y cada elemento de un tipo compuesto recibe su respectivo valor cero. El valor cero de un tipo compuesto no es `nil`, sino una instancia válida donde todos sus componentes tienen sus valores cero correspondientes.

Es importante entender que el valor cero hace que todas las variables estén en un estado definido y usable inmediatamente después de su declaración, sin necesidad de inicialización explícita.

### Inicialización de un paquete

Dentro de un paquete, la inicialización de variables a nivel de paquete ocurre paso a paso. En cada paso se selecciona la variable declarada más temprano que esté lista para inicialización (no tenga dependencias no resueltas).

Una variable a nivel de paquete está lista para inicialización si:
- No ha sido inicializada aún,
- No tiene expresión de inicialización, o
- Su expresión de inicialización no depende de variables aún no inicializadas

Este proceso continúa hasta que no queden variables por inicializar. Si al finalizar quedan variables sin inicializar, significa que forman parte de un ciclo de dependencias, lo cual hace que el programa sea inválido.

El orden de declaración de variables entre diferentes archivos del mismo paquete está determinado por el orden en que los archivos se presentan al compilador. Los sistemas de construcción deben presentar los archivos en orden lexicográfico por nombre para garantizar comportamiento reproducible.

El análisis se basa únicamente en referencias léxicas (sintácticas) a identificadores, no en valores en tiempo de ejecución. Solo se consideran referencias a variables, funciones y métodos declarados en el mismo paquete, las referencias a otros paquetes no crean dependencias de inicialización.

Las variables también pueden ser inicializadas mediante funciones `init` declaradas a nivel de paquete. Estas funciones:
- No pueden tener parámetros ni valores de retorno
- Se pueden declarar múltiples por paquete y por archivo
- Solo pueden ser declaradas, no invocadas explícitamente
- Se ejecutan después de que todas las variables estén inicializadas

Un paquete se considera completamente inicializado cuando:
- Todas sus variables a nivel de paquete tienen valores asignados
- Todas las funciones `init` han sido ejecutadas en el orden que aparecen en el código fuente

### Inicialización de un programa

Los paquetes de un programa completo se inicializan paso a paso, un paquete a la vez. Si un paquete tiene importaciones, todos los paquetes importados se inicializan completamente antes que el paquete que los importa. Si un paquete es importado por múltiples paquetes, se inicializa exactamente una vez. Este diseño garantiza que no hay duplicación de inicialización ni ciclos de inicialización entre paquetes.

La inicialización del programa completo ocurre en una sola rutina go, de manera secuencial. Aunque las funciones `init` pueden crear nuevas rutinas go, el proceso de inicialización espera a que todas las funciones `init` del paquete actual terminen antes de continuar con el siguiente paquete.

### Ejecución de un programa

Un programa ejecutable se crea enlazando un paquete especial llamado `main package` con todos los paquetes que importa directa o indirectamente. Este paquete debe:
- Tener el nombre de paquete `main`
- Declarar una función llamada `main` que no reciba parámetros ni retorne valores

La ejecución del programa sigue esta secuencia:
- Inicialización completa del programa: todos los paquetes se inicializan en orden de dependencias
- Invocación de `main()`: se llama a la función `main` del paquete `main`
- Terminación: cuando `main()` retorna, el programa termina inmediatamente sin esperar a que otras rutinas go finalicen

## Errores

El tipo predeclarado `error` es una interfaz que representa la forma convencional de manejar condiciones de error en Go. Cualquier valor que implemente esta interfaz puede representar un error, donde `nil` indica ausencia de error y cualquier valor `no-nil` indica la presencia de un error.
```Go
type error interface {
    Error() string
}
```

La interfaz `error` requiere únicamente un método `Error()` que retorne una representación `string` del error. Esta simplicidad permite que cualquier tipo pueda implementar la interfaz `error` definiendo este método.

El diseño de Go favorece el manejo explícito de errores mediante valores de retorno, en lugar de excepciones. El patrón idiomático es retornar un error como último valor de retorno de una función, permitiendo al código llamador decidir cómo manejar cada condición de error.

## Pánicos en tiempo de ejecución

Los errores que ocurren durante la ejecución del programa, como el uso de un índice fuera de los límites de un arreglo o slice, desreferencia de un puntero nil, o división por cero, activan un pánico en tiempo de ejecución.

Un pánico en tiempo de ejecución es equivalente a llamar explícitamente a la función `panic` con un valor que implementa la interfaz predeclarada `error`. Específicamente, estos pánicos generalmente contienen un valor de tipo que pertenece al paquete `runtime` (como `runtime.Error`) que describe la naturaleza del error de ejecución.

Cuando ocurre un pánico en tiempo de ejecución, el programa sigue la misma secuencia que un pánico explícito: la función actual se detiene, se ejecutan las funciones defer, y el pánico se propaga hacia arriba en la pila de llamadas hasta que es recuperado con `recover` o el programa termine.

## Consideraciones de sistema

### Paquete unsafe

El paquete `unsafe` es integrado y reconocido por el compilador. Proporciona facilidades para programación de bajo nivel, incluyendo operaciones que pueden violar el sistema de tipos de Go. Los paquetes que usen `unsafe` requieren gestión manual cuidadosa, ya que pueden no ser portables entre diferentes arquitecturas o versiones del compilador.

Este paquete ofrece las siguientes interfaces:
```Go
package unsafe
type ArbitraryType int    // placeholder para cualquier tipo de Go; no es un tipo real
type Pointer *ArbitraryType
func Alignof(variable ArbitraryType) uintptr
func Offsetof(selector ArbitraryType) uintptr
func Sizeof(variable ArbitraryType) uintptr
type IntegerType int      // placeholder para tipos enteros; no es un tipo real
func Add(ptr Pointer, len IntegerType) Pointer
func Slice(ptr *ArbitraryType, len IntegerType) []ArbitraryType
func SliceData(slice []ArbitraryType) *ArbitraryType
func String(ptr *byte, len IntegerType) string
func StringData(str string) *byte
```

### Garantías de tamaño y alineación

Para tipos numéricos, Go garantiza los siguientes tamaños:
- **1 byte:** `byte`, `uint8`, `int8`
- **2 bytes:** `uint16`, `int16`
- **4 bytes:** `uint32`, `int32`, `float32`
- **8 bytes:** `uint64`, `int64`, `float64`, `complex64`
- **16 bytes:** `complex128`

Además, las garantías de alineación mínima son:
- **Cualquier variable:** alineación mínima de 1 byte
- **Variables de tipo struct:** alineación igual al mayor requerimiento de alineación de sus campos
- **Variables de tipo arreglo:** alineación igual a la alineación del tipo de sus elementos

Estas garantías permiten escribir código que dependa de representaciones específicas de memoria cuando sea absolutamente necesario.

# Sección 4: Effective Go

## Formateo

Un problema recurrente en programación es la inconsistencia en estilos de código. Go resuelve esto delegando el trabajo de formateo a herramientas automáticas, eliminando debates sobre preferencias personales.

El programa `gofmt` (o `go fmt` como comando integrado) formatea código Go de manera automática y consistente. Opera a nivel de paquete, asegurando que todos los archivos en un paquete mantengan el mismo estilo, en lugar de formatear archivos de forma aislada.

`gofmt` no siempre es "perfecto" en el sentido de que puede no alinearse con las preferencias personales de estilo, pero su propósito no es complacerlas, sino imponer un estándar consistente a nivel de paquete.

Los siguientes son los aspectos que `gofmt` normaliza:
- **Indentación:** usa tabs por defecto en lugar de espacios
- **Espacios en blanco:** ajusta espacios en expresiones, alineación de campos y comentarios
- **Paréntesis:** mantiene solo la menor cantidad necesaria 
- **Alineación:** alinea elementos para mejorar legibilidad
- **Longitud de línea:** Go no impone una longitud máxima de línea estándar

Ejemplo:
- Antes de usar `go fmt`:
    ```Go
    type T struct {
        nombre string // Comentario 1
        edad int // Comentario 2
    }
    ```
- Usar el programa para formatear el código:
    ```bash
    go fmt .
    ```
- Después de usar `go fmt`:
    ```go
    type T struct {
        nombre string // Comentario 1
        edad   int    // Comentario 2
    }
    ```

## Comentarios

Go soporta comentarios de bloque al estilo C (`/* */`) y comentarios de una sola línea (`//`). Los comentarios de una línea son la norma; los de bloque se usan típicamente para comentarios de paquete o para desactivar grandes bloques de código.

Todo comentario que aparezca inmediatamente antes de una declaración (sin líneas en blanco intermedias) se convierte en comentario de documentación para esa declaración. Estos forman la documentación primaria de un paquete. Sin embargo, solo las declaraciones exportadas (que comienzan con letra mayúscula) generan documentación pública. Las no exportadas también pueden tener comentarios de documentación, pero solo son visibles internamente.

Además, existen herramientas como `godoc` o `go doc`, que procesan automáticamente estos comentarios y genera documentación accesible desde diversos lugares (terminal, web, IDEs, etc.).

**Convenciones de comentarios de documentación:**
- **Empezar con el nombre:** Debe comenzar con el nombre de lo que está documentando
- **Oración completa:** Debe terminar con punto final
- **Conciso y descriptivo:** Debe explicar el propósito, no el código
- **Múltiples párrafos:** Debe usar comentarios de una línea (`//`) y separar las explicaciones con comentarios en blanco

## Nombres

Los nombres en Go tienen efecto semántico: la visibilidad de un nombre fuera de su paquete está determinada por su primer carácter (mayúscula = exportado, minúscula = no exportado).

### Nombres de paquetes

Cuando un paquete se importa, su nombre se convierte en un identificador calificado para acceder a su contenido exportado.

**Convenciones para nombres de paquetes:**
- Deben estar en **minúsculas**, ser de **una sola palabra** y no **sin guiones bajos**
- No necesitan ser únicos globalmente; si hay colisiones, asigna un alias local
- El nombre del paquete corresponde a la **última parte de la ruta**: `encoding/base64` se importa como tal, pero el nombre es `base64`

La ventaja de estas convenciones es que el nombre del paquete proporciona contexto claro. Por ejemplo, múltiples paquetes pueden exportar `Reader` sin conflicto: `io.Reader` vs `bufio.Reader` son distintos.

### Getters y Setters

Go no proporciona soporte automático para getters/setters porque no es idiomático. En su lugar, usa el sistema de visibilidad (mayúsculas/minúsculas) para control explícito.

Por ejemplo, para exponer un campo privado de forma controlada, se crea un método con el mismo nombre pero con su primer caracter en mayúsculas.

Ejemplo:
```go
type Usuario struct {
    nombre string // privado
}

// Getter idiomático (sin prefijo "Get")
func (u *Usuario) Nombre() string {
    return u.nombre
}

// Setter
func (u *Usuario) SetNombre(n string) {
    u.nombre = n
}
```

### Nombres de interfaces

Por convención, las interfaces se nombran con el nombre de su(s) método(s) más el sufijo `er`:

Ejemplo:
```go
type Reader interface {
    Read(p []byte) (n int, err error)
}

type Writer interface {
    Write(p []byte) (n int, err error)
}
```

Para interfaces compuestas, se concatenan los nombres de las interfaces existentes.

Ejemplo:
```go
type ReadWriter interface {
    Reader
    Writer
}

type ReadCloser interface {
    Reader
    Closer
}
```

### MixedCaps

La convención de Go para nombres es usar **MixedCaps** (mezcla de mayúsculas y minúsculas), evitando guiones bajos.

- **Mayúscula inicial** (`MixedCaps`): exportado fuera del paquete
- **Minúscula inicial** (`mixedCaps`): no exportado, solo visible dentro del paquete

## Punto y Coma

Al igual que C, la gramática formal de Go utiliza el punto y coma `;` para finalizar las sentencias, pero no aparecen en el código. En su lugar, el analizador léxico sigue una regla para insertar el punto y coma automáticamente al escanear el código fuente.

**Regla:** Si el último token antes de una nueva línea es un identificador, una literal básica o uno de los tokens `break`, `continue`, `fallthrough`, `return`, `++`, `--`, `)`, `}`, el analizador léxico siempre insertará un punto y coma inmediatamente después de dicho token.

Esta regla se resume como: "Si la nueva línea está después de un token que podría finalizar una sentencia, se agrega un punto y coma".

Programas idiomáticos de Go prácticamente no tienen puntos y comas, únicamente en lugares donde verdaderamente marcan una diferencia, como en bucles `for` (con sus tres partes) o múltiples sentencias en una sola línea.

Una consecuencia de la regla para insertar puntos y coma es que no se puede poner la llave de apertura de una sentencia en una nueva línea, pues se insertaría un punto y coma y el comportamiento se vería afectado.

Ejemplo:
- Forma correcta:
    ```go
    if i < f() {
        g()
    }
    ```

- Forma incorrecta:
    ```go
    if i < f() 
    {
        g()
    }
    ```

En el segundo caso, se inserta `;` después de `f()`, dejando las llaves desligadas de la condición.

## Estructuras de Control

Las estructuras de control en Go están relacionadas con las de C, pero difieren en puntos importantes. Go no requiere paréntesis en la sintaxis de estructuras de control, pero sus cuerpos **deben estar siempre entre llaves**.

**Características generales:**
- No hay bucles `while` o `do while`, solo un bucle `for` generalizado
- Tanto `if` como `switch` aceptan una sentencia de inicialización opcional, similar a la de `for`
- Las sentencias `break` y `continue` aceptan etiquetas opcionales para identificar su acción
- Nueva estructura de control: `select`

### If

Un simple `if`:
```go
if x > 0 {
    return y
}
```

Con inicialización (la variable existe solo dentro de su bloque if):
```go
if err := file.Chmod(0664); err != nil {
    log.Print(err)
    return err
}
```

Las llaves obligatorias fomentan sentencias simples en múltiples líneas. Es común omitir `else` en sentencias `if` que limitan el flujo, ya que resulta innecesario.

### Re-declaración y re-asignación

En declaraciones cortas (`:=`) dentro del mismo bloque, se pueden mezclar variables nuevas y existentes. Las nuevas se **declaran**, mientras que las existentes se **reasignan**:
```go
if err := someFunc(); err != nil {
    f, err := os.Open("file")  // f se declara, err se reasigna aquí
    // ...
}
```

Esto es idiomático y reduce la necesidad de nuevos nombres de variables, especialmente útil para variables como `err`.

### For

La sentencia `for` generaliza todos los bucles, y puede tomar tres formas:
- **Forma completa:**
    ```go
    for pre; condición; post { }
    ```
- **Forma while (solo condición):**
    ```go
    for condición { }
    ```
- **Forma infinita:**
    ```go
    for { }
    ```

La palabra reservada `range` gestiona bucles sobre arreglos, slices, strings, mapas o canales, y devuelve valores según el tipo:
- **Slice/Arreglo**: índice y valor
- **Mapa**: clave y valor
- **String**: índice (posición de byte) y rune
- **Canal**: solo valor

Es posible descartar valores con el identificador en blanco `_` o no asignarlos cuando no se necesitan:
```go
for indice, valor := range slice { }
for _, valor := range slice { }       // descarta índice
for indice := range array { }         // solo índice
for valor := range canal { }          // solo valor (canal)
```

### Switch

La sentencia `switch` es más general que en C, sin embargo, las expresiones no deben ser constantes o enteros, y los casos se evalúan de arriba hacia abajo hasta que uno se cumple. Si no hay una expresión, se toma como `true`:
```go
switch variable {
case "valor1":
    return true
case "valor2":
    return false
default:
    return false
}
```

Además **no hay fall through automático**, pero se pueden agrupar múltiples casos separados por comas:
```go
switch c {
case ' ', '?', '&', '=':
    return true
}
```

O, si es necesario forzar fall through entre casos, se debe usar la palabra reservada `fallthrough`:
```go
switch x {
case 1:
    fmt.Println("uno")
    fallthrough
case 2:
    fmt.Println("dos")
}
```

### Switch de tipo

La sentencia `switch` también puede descubrir el tipo dinámico de una variable de tipo interfaz usando la sintaxis parecida a una aserción de tipo, pero con la palabra reservada `type`:
```go
switch t := t.(type) {
case bool:
    return "booleana"
case string:
    return "string"
case int:
    return "int"
default:
    return "inesperado"
}
```

La reasignación `t := t.(type)` permite usar `t` con su tipo específico en cada uno de los casos.

## Funciones

### Múltiples valores de retorno

Go permite que funciones y métodos retornen múltiples valores en una sola llamada. Por lo tanto, el patrón idiomático para manejo de errores es retornar el resultado seguido de un objeto tipo `error` como último valor. Esto evita prácticas raras como devolver -1 o EOF para indicar error.

Ejemplo:
```go
func Open(name string) (*File, error) {
    // ...
}
```

### Parámetros nombrados de resultado

Los valores de retorno pueden tener nombres, al igual que variables normales. Cuando están nombrados, se inicializan con su **valor cero** al inicio de la función, y, si la función retorna sin especificar valores, se usan automáticamente los parámetros nombrados. Nombrar los valores de retorno no es obligatorio, pero mejora la claridad y sirve como documentación.

Ejemplo:
```go
func ReadFull(r Reader, buf []byte) (n int, err error) {
    for len(buf) > 0 {
        nn, e := r.Read(buf)
        if e != nil {
            err = e
            break
        }
        n += nn
        buf = buf[nn:]
    }
    return  // retorna "n" y "err" automáticamente
}
```

### Defer

La sentencia `defer` programa una función para que se ejecute inmediatamente antes de que la función actual finalice o retorne. Es útil para liberar recursos o ejecutar acciones independientemente del flujo.

Los argumentos de la función diferida se evalúan **cuando `defer` se ejecuta, no cuando la función se ejecuta**. Esto provoca que los valores se "congelen". Además, las funciones defer se ejecutan en orden **LIFO** (Last-In, First-Out).

Ejemplo:
```go
for i := 0; i < 3; i++ {
    defer fmt.Println(i)  // congelará 0, 1, 2
}
// Imprime: 2, 1, 0 (orden LIFO)
// Sin congelación, todas las llamadas imprimirían 3

```

**Otras características:**
- Un `return` dentro de una función defer no afecta el retorno de la función que la contiene
- Para manejar panics, usa `recover()` dentro de un `defer`

## Datos

### Asignación con new

Go tiene dos funciones integradas para la asignación de memoria: `new` y `make`. La función `new` asigna memoria para cierto tipo, la inicializa con su valor cero correspondiente y retorna su dirección.

Debido a que la memoria asignada contiene valores cero (zeroed), está lista para usar sin inicialización adicional.

### Constructores y literales compuestas

A veces asignar un valor cero no es suficiente, por lo que un constructor inicializador hace que el espacio de memoria sea usable.

Ejemplo tradicional:
```go
func NewFile(fd int, name string) *File {
    if fd < 0 {
        return nil
    }
    f := new(File)
    f.fd = fd
    f.name = name
    f.dirinfo = nil
    f.nepipe = 0
    return f
}
```

Las **literales compuestas** logran lo mismo de forma más concisa: crean una nueva instancia y asignan valores simultáneamente.
```go
func NewFile(fd int, name string) *File {
    if fd < 0 {
        return nil
    }
    return &File{fd, name, nil, 0}
}
```

Los campos se asignan en orden de declaración o por nombre, y los campos omitidos toman su valor cero. En Go, es válido retornar la dirección de una variable local, pues el **escape analysis** del compilador detecta variables usadas fuera de su scope y las coloca en memoria que persiste tras el return de la función.

### Asignación con make

La función `make` solo funciona con slices, mapas y canales, retornando el valor completamente inicializado (no un puntero). A diferencia de `new`, `make` inicializa los metadatos internos requeridos por estas estructuras:
- **Slices**: inicializa el descriptor (puntero, longitud, capacidad)
- **Mapas**: inicializa la tabla hash interna
- **Canales**: inicializa el buffer y sincronización

### Arreglos

Los arreglos son útiles cuando se necesita control detallado de memoria o garantizar tamaño fijo. Sus principales características son:
- Se copian completos al asignarlos (por valor)
- Al pasarlos a funciones, se recibe una copia, no un puntero
- El tamaño es parte del tipo: `[3]int` y `[4]int` son tipos diferentes

En la mayoría de casos, usa slices en lugar de arreglos, pues usar punteros a arreglos no es idiomático en Go.

### Slices

Los slices envuelven arreglos para proporcionar una interfaz más general, poderosa y conveniente, y en la mayoría de casos, se prefiere usar slices sobre arreglos.

Un slice contiene una referencia a un arreglo subyacente, incluso, múltiples slices pueden compartir el mismo arreglo subyacente.

- **Longitud** (`len`): elementos actuales
- **Capacidad** (`cap`): máxima longitud del arreglo subyacente

Si un slice sobrepasa su capacidad, se reasigna el arreglo subyacente.

### Slices de dos dimensiones

Los arreglos y slices en Go son unidimensionales. Para 2D, es necesario crear arreglos de arreglos o slices de slices:

```go
type Transform [3][3]float64  // Array 3x3 (tamaño fijo)
type LinesOfText [][]byte     // Slice de slices (dinámico)
```

### Mapas

Un mapa asocia valores de un tipo (clave) con valores de otro tipo. La clave puede ser cualquier tipo con `==` definido: enteros, strings, punteros, etc. Los slices no pueden ser claves (no tienen `==`).

Los mapas se usan por referencia, y pueden ser construidos con literales compuestas:
```go
m := map[string]int{"a": 1, "b": 2}
```

Acceder a una clave inexistente devuelve el valor cero del tipo. Entonces, para distinguir entre "clave ausente" y "clave presente con valor cero", se usa la sintaxis **"comma ok"**:
```go
m := map[string]int{"a": 0}
v, ok := m["a"]      // v = 0, ok = true
v, ok := m["inexistente"]  // v = 0, ok = false
```

Sin `ok`, ambos casos darían el mismo resultado.

Para borrar una entrada, usa `delete(mapa, clave)`, esto es seguro incluso si la clave no existe.

### Imprimir

El paquete `fmt` proporciona funciones para imprimir con formato.

### Append

La función integrada `append` agrega elementos al final de un slice y retorna el resultado:
```go
func append(slice []T, elements ...T) []T
```

El arreglo subyacente puede cambiar si se sobrepasa la capacidad. Por ello, **se debe reasignar el resultado**:
```go
s := []int{1, 2}
s = append(s, 3, 4)  // reasignación necesaria
```

## Inicialización

La inicialización en Go es más poderosa que en otros lenguajes. Estructuras complejas se construyen durante la inicialización, y los problemas de orden entre objetos e incluso paquetes se gestionan correctamente de forma determinística.

### Constantes

Las constantes son exactamente eso: constantes. Se crean en tiempo de compilación incluso si se definen dentro de funciones. Solo pueden ser números, caracteres (runas), strings o booleanos, ya que estos tipos se pueden computar completamente en tiempo de compilación. Las expresiones que las definen también deben ser constantes.

Las constantes enumeradas pueden ser creadas con `iota`, que asigna valores consecutivos:
```go
const (
    A = iota    // 0
    B           // 1 (hereda iota del anterior)
    C = iota    // 2 (iota sigue incrementando)
    D           // 3 (hereda iota)
)
```

**Comportamiento clave:**
- `iota` comienza en 0 al inicio de cada bloque `const`
- Dentro del mismo bloque, `iota` incrementa en cada línea
- Si una línea no usa `iota` explícitamente, hereda el valor anterior
- Si múltiples constantes están en la misma línea, todas toman el mismo valor de `iota`

```go
const (
    A = iota    // 0
    B, C        // 1, 1 (misma línea, mismo iota)
    D           // 2
)
```

### Variables

Las variables se inicializan como constantes, pero sus expresiones y valores se crean en tiempo de ejecución:
```go
var (
    home   = os.Getenv("HOME")
    user   = os.Getenv("USER")
    gopath = os.Getenv("GOPATH")
)
```

### La función init

Cualquier archivo puede definir funciones niládicas (sin argumentos) llamadas `init` para configurar estado. Incluso, un archivo puede tener múltiples funciones `init`, y se ejecutan en orden textual (orden en que aparecen en el código).
```go
func init() {
    // configuración inicial
}
```

Las funciones `init` se ejecutan una vez que:
1. Todos los paquetes importados han sido inicializados
2. Todas las declaraciones de variables del paquete han sido evaluadas

Un uso común de `init` es verificar, reparar o asegurar que el estado del programa sea correcto antes de la ejecución real.

## Métodos

### Punteros vs. Valores

Los métodos pueden definirse para cualquier tipo nombrado (excepto punteros e interfaces). Un método es una función con un **receiver**, que es el tipo sobre el cual opera.
```go
type ByteSlice []byte

func (slice ByteSlice) Append(data []byte) []byte {
    // slice es el receiver por valor
    return append(slice, data...)
}
```
La diferencia principal es si el método puede modificar el original:

**Receiver por valor:** Pueden invocarse en valores y punteros

```go
func (slice ByteSlice) Append(data []byte) []byte {
    // Recibe una COPIA de ByteSlice
    // No puede modificar el original
    // Debe retornar el resultado
    return append(slice, data...)
}
```

**Receiver por puntero:** Solo pueden invocarse en punteros
```go
func (p *ByteSlice) Append(data []byte) {
    // Recibe la DIRECCIÓN de ByteSlice
    // Puede modificar el original directamente
    slice := *p
    slice = append(slice, data...)
    *p = slice  // Modifica el original
}
```

Esto previene un error común, pues si permitiera invocar un método de puntero en un valor, recibiría una copia y las modificaciones se perderían.

Si el valor es **addressable** (tiene una dirección de memoria), el compilador convierte automáticamente un método de puntero invocado en un valor. Esto solo ocurre para valores addressables (variables, no resultados de expresiones).

## Interfaces y otros tipos

### Interfaces

Las interfaces en Go especifican el comportamiento de un objeto: si algo puede hacer esto, puede ser usado aquí.

Un tipo implementa una interfaz si tiene todos sus métodos. **Go usa implementación implícita**, pues no hay palabra clave para este comportamiento. El compilador verifica automáticamente si un tipo satisface una interfaz.

Un único tipo puede implementar múltiples interfaces.

### Conversiones

Existen dos tipos de conversiones legales:

**Conversiones sin crear nuevo valor:** Ocurren entre tipos que el compilador considera equivalentes. Solo cambian la "etiqueta" del tipo
```go
type MyInt int
var x MyInt = 5
y := int(x)  // No crea nuevo valor, solo cambia el tipo
```

**Conversiones que crean nuevo valor:** Ocurren entre tipos distintos que sí requieren algún cálculo
```go
var x int = 3
y := float64(x)  // Crea un nuevo valor
```

En Go, es idiomático convertir un tipo a otro para acceder a métodos diferentes, reduciendo así la cantidad de métodos que un solo tipo debe implementar.

### Conversión de interfaces y aserción de tipos

Los **switches de tipo** toman una interfaz y la convierten al tipo de cada caso. Son útiles cuando se espera trabajar con interfaces que pueden tener múltiples tipos.
```go
switch v := i.(type) {
case int:
    // v es int
case string:
    // v es string
}
```

Por otro lado, las **aserciones de tipo** extraen un valor de tipo interfaz y lo convierten a un tipo específico. Resulta más conveniente cuando solo interesa un tipo.
```go
str, ok := i.(string)  // Notación "comma, ok" segura
```

Si una aserción de tipo falla sin usar `comma, ok`, ocurre un error en tiempo de ejecución. Con `comma, ok`, si la aserción falla:
- El valor convertido toma su valor cero
- La variable `ok` será `false`

### Generalidad

Cuando un tipo existe únicamente para implementar una interfaz sin agregar comportamiento adicional, exportar el tipo es innecesario. En su lugar, es recomendable hacer lo siguiente:
- Mantener el tipo **privado** (minúscula)
- Exportar la **interfaz** (mayúscula)
- Los constructores deben retornar la interfaz, no el tipo concreto

Ejemplo:
```go
// Privado
type byteWriter struct { /* ... */ }

// Pública
type Writer interface {
    Write(p []byte) (n int, err error)
}

// Constructor retorna interfaz
func NewWriter() Writer {
    return &byteWriter{}
}
```

Esto deja claro que el comportamiento (la interfaz) es lo importante.

### Interfaces y métodos

Prácticamente cualquier tipo nombrado puede tener métodos. Los únicos que **no pueden** tener métodos son:
- **Punteros**: sería redundante (`*(*T)`)
- **Interfaces**: ya son abstractas; métodos en interfaces de interfaces no tiene sentido

Esto significa que casi cualquier tipo puede satisfacer una interfaz.

## El identificador en blanco

El identificador en blanco (`_`) es una variable especial que descarta cualquier valor de cualquier tipo sin consecuencias. Se usa para cumplir requisitos sintácticos sin crear variables innecesarias.

### El identificador en blanco en asignaciones múltiples

Cuando una asignación múltiple produce valores que no serán usados, usar `_` evita crear variables innecesarias y deja explícito que el valor se descarta:
```go
// for range
for _, valor := range slice {
    // descarta el índice
}

// Canales
_, ok := <-canal  // descarta el valor, verifica si hay más

// Aserciones de tipo
_, ok := i.(string)  // descarta el valor, verifica que es string
```

### Importaciones y variables sin usar

En Go, importar un paquete o declarar una variable que no se usa es un **error de compilación**. Esto evita código muerto y acelera la compilación.

Durante desarrollo temprano, cuando se sabe que se usará un paquete pero aún no lo es, es una buena práctica silenciar el error con `_`:
```go
import (
    "fmt"
    "log"  // Sin usar aún
)

var _ = log.Printf  // Silencia el error de compilación
```

La convención es que estas líneas deben estar justo después de la importación y comentadas para recordar corregirlas.

### Importar para efectos secundarios

A veces es necesario importar un paquete solo por sus efectos secundarios (inicialización, registro, etc.) sin usarlo directamente, por lo que se usa `_` como nombre local:
```go
import _ "net/http/pprof"
```

En este caso, cuando `pprof` se importa, registra automáticamente un servidor HTTP (efecto secundario). El `_` deja claro que el paquete se importa únicamente por este efecto.

### Chequeo de interfaces

Para verificar en **tiempo de compilación** que un tipo implementa una interfaz, es posible usar una aserción de tipo con `_`:
```go
var _ io.Writer = (*MyWriter)(nil)
```

Si `MyWriter` no implementa todos los métodos de `io.Writer`, esto produce error de compilación. Es útil como documentación y verificación automática.

```go
// Verificar que múltiples tipos implementan Reader
var _ io.Reader = (*File)(nil)
var _ io.Reader = (*Buffer)(nil)
```

## Embeber

Go usa **composición** en lugar de herencia. Embeber permite "tomar prestado" implementaciones existentes al embeber tipos dentro de structs o interfaces.

Para embeber interfaces, se debe especificar la interfaz dentro de otra. Solo es posible embeber interfaces en interfaces:
```go
type Reader interface {
    Read(p []byte) (n int, err error)
}

type Writer interface {
    Write(p []byte) (n int, err error)
}

type ReadWriter interface {
    Reader  // Embebe Reader
    Writer  // Embebe Writer
}
```

`ReadWriter` puede hacer lo que `Reader` y `Writer` hacen, formando una **unión de interfaces**.

Si la misma interfaz se embebe indirectamente (a través de otras), los métodos solo necesitan satisfacerse una vez.

Para embeber structs, la sintaxis es similar a declarar un campo, pero sin declarar un nombre:
```go
type Reader struct {
    // ...
}

type Writer struct {
    // ...
}

type ReadWriter struct {
    *Reader  // Embebe puntero a Reader
    *Writer  // Embebe puntero a Writer
}
```

**Diferencia entre valor y puntero:**
- Embeber `Reader`: siempre existe con zero values
- Embeber `*Reader`: puede ser `nil`

Al embeber, tanto **campos como métodos** del tipo interno se promocionan al tipo externo:
```go
type Inner struct {
    X int
}

func (i *Inner) Method() {
    i.X++
}

type Outer struct {
    Inner
}

o := Outer{Inner{5}}
o.X = 10        // acceso directo al campo embebido
o.Method()      // llamada directa al método embebido
```

Cuando se invoca un método embebido, el **receiver sigue siendo el tipo interno**, lo que asegura comportamiento correcto y esperado:
```go
type Inner struct{ x int }
func (i *Inner) Increment() { i.x++ }

type Outer struct{ Inner }

o := Outer{Inner{5}}
o.Increment()  // receiver es Inner, no Outer
// o.Inner.x ahora es 6
```

La capacidad de embeber en Go introduce un problema, siendo la duplicación de nombres. Cuando hay duplicación de nombres, se aplican dos reglas:

**Regla 1: Ocultamiento por nivel**
Un campo o método X en el nivel externo oculta cualquier X en niveles internos:
```go
type Inner struct{ X int }
type Outer struct {
    Inner
    X string  // Oculta Inner.X
}

o := Outer{}
o.X         // string (nivel externo)
o.Inner.X   // int (acceso explícito)
```

**Regla 2: Conflictos al mismo nivel**
Si el mismo nombre aparece en el mismo nivel de anidación, es un error **solo si se usa**. Si nunca se menciona, está permitido:
```go
type A struct{ X int }
type B struct{ X int }
type C struct {
    A
    B
    // Ambos tienen X al mismo nivel
}

c := C{}
// c.X   // ERROR: ambiguo
c.A.X    // OK: acceso explícito
```

Esto evita errores innecesarios en código que funciona sin acceder a campos conflictivos.

## Concurrencia

## Referencias

- ["Documentation"](https://go.dev/doc/)
- ["A Tour of Go"](https://go.dev/tour)
- ["How to Write Go Code"](https://go.dev/doc/code)
- ["The Go Programming Language Specification"](https://go.dev/ref/spec)
- ["Effective Go"](https://go.dev/doc/effective_go)
