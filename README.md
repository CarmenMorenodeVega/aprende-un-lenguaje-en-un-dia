# Aprende un lenguaje de programación en un día (ejercicio voluntario para subir nota).

## Miembros del grupo

* Carmen Moreno de Vega
* Manuel Zambrana
* Adrian Sánchez

## Lenguaje de programación

El profesor llevará una cajita llena de papelitos con los nombres de distintos lenguajes de programación. Los encargados de cada grupo meterán la mano en la caja y sacarán dos papelitos, de los cuales el grupo elegirá uno. Se permite hacer intercambio de papelitos entre grupos.

Escribe el lenguaje de programación elegido .

* El lenguaje elegido por el grupo RUSTPOWER es RUST por ser un lenguaje en auge.

## Información sobre el lenguaje

Aunque muchos están conociendo el lenguaje RUST en los últimos años, oficialmente salió a la luz en el 2010.
Los proyectos desarrollados con Rust pueden dividirse en cliente y servidor, cualidad que hace que Rust sea uno de los lenguajes más querido por los desarrolladores.

Compañías como Coursera, Dropbox, NPM y otros están empezando a utilizar Rust en sus proyectos. Dropbox, por ejemplo, lo esta usando en sus clientes de Windows, así que ya tenemos millones de implementaciones que están usando Rust y NPM lo esta utilizando para el trabajo con paquetes de Javascript.

Las características más importantes de este lenguaje son:

1. Rust es un lenguaje con una sintaxis es muy similar a C y C++, es decir que estaríamos encontrando las clásicas llaves y bloques de código como las condicionales y los ciclos. 

2. Para las variables RUST es capaz de deducir tipos, así que no siempre le tendremos que decir que tipo de dato es, pero para que esto se aplique tendremos que utilizar la palabra'let'. Para permitir que una variable sea mutable tendremos que agregar la palabra 'mut' a la palabra 'let' en la definición de la variable.

3. Rust no nos permite, como ya lo hacen ahora muchos lenguajes, utilizar un valor que no haya sido inicializado previamente. Algo que también se repite en otros lenguajes de programación es que al menos necesitamos una función de inicio (la famosa función main). Ahora viene una característica importante, Rust es un lenguaje basado en expresiones, de hecho existen 2 tipos de sentencias y todo lo demás son solo una expresión.

## Herramientas de desarrollo

Para comenzar a utilizar este lenguaje es necesario descargarse la aplicación "rustup-init" e instalarla. en cuadnto a la IDE requerida para editar y visualizar el programa

## Poniendo en práctica el lenguaje

Pon en práctica el lenguaje de programación realizando los siguientes ejercicios. Para cada uno de los ejercicios, pega el código fuente de la solución y una captura de pantalla.

### 1. ¡Hola mundo!
Escribe por pantalla "Hola mundo".
```rust
fn main(){
  println!("Hola mundo");
}
```



### 2. Pirámide

Dada una altura introducida por el usuario, realiza un programa que pinte una pirámide a base de asteriscos con la altura indicada.

```rust
use std::io;
use std::io::Write;
use std::str::FromStr;
use std::num::ParseIntError;
 
fn read_input() -> Result<u32,ParseIntError> {
    print!("Dime la altura de la pirámide: ");
    io::stdout().flush().ok();
    let mut input = String::new();
    io::stdin().read_line(&mut input).ok().expect("Error al leer de teclado");
    let input = input.trim();
    let altura: u32 = u32::from_str(&input)?;
    Ok(edad)
}
 
fn main() {
    let altura;
    let mut bucle=0;
    let mut asteriscos=1;
    loop {
        if let Ok(e) = read_input(){
            altura = e;
            break;
        }
        else{
            println!("Introduce un numero, por favor");
        }
    }
    
    let mut  espacios = altura + 1;
    
    while bucle < altura {
    	for _x in 1..espacios {
    		print!(" ");	
    	}
    	
      for _x in 0..asteriscos {
    		print!("*");
    	}
    	
      println!("");
    	bucle+=1;
    	asteriscos+=2;
    	espacios-=1;
    	
    }
}
```

### 3. Arrays y números aleatorios

Realiza un programa que rellene un array (o una estructura similar) con 20 números enteros aleatorios entre 1 y 100 y que seguidamente los muestre por pantalla. A continuación, se deben pasar los números primos a las primeras posiciones del array y los no primos a las posiciones restantes. Muestra finalmente el array resultado.

```rust

```


Si te ha gustado este lenguaje y la exposición, dale una estrellita al [repositorio original](https://github.com/CarmenMorenodeVega/aprende-un-lenguaje-en-un-dia).

