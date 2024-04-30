# ejemplo_poo


```javascript

    // Clase Libro
    class Libro {
      constructor(titulo, autor, editorial, año) {
        this.titulo = titulo;
        this.autor = autor;
        this.editorial = editorial;
        this.año = año;
      }

      mostrarInfo() {
        return `Título: ${this.titulo}\nAutor: ${this.autor}\nEditorial: ${this.editorial}\nAño: ${this.año}`;
      }
    }

    // Crear objetos Libro
    const libro1 = new Libro("Cien años de soledad", "Gabriel García Márquez", "Sudamericana", 1967);
    const libro2 = new Libro("Orgullo y Prejuicio", "Jane Austen", "Penguin Classics", 1813);
    const libro3 = new Libro("El Señor de los Anillos", "J.R.R. Tolkien", "Allen & Unwin", 1954);

    // Obtener el elemento del DOM donde se mostrarán los libros
    const divLibros = document.getElementById("libros");

    // Mostrar la información de los libros en la página
    divLibros.innerHTML = `
      <p>${libro1.mostrarInfo()}</p>
      <p>${libro2.mostrarInfo()}</p>
      <p>${libro3.mostrarInfo()}</p>
    `;

```
## Explicación del código:

1. Se define una clase llamada Libro que tiene un constructor que recibe los datos del libro (título, autor, editorial y año) y los almacena como propiedades del objeto.
2. La clase Libro también tiene un método mostrarInfo() que devuelve una cadena con la información del libro.
3. Se crean tres objetos Libro con diferentes valores para sus propiedades.
4. Se obtiene el elemento del DOM donde se mostrarán los libros y se usa el método mostrarInfo() de cada objeto para mostrar 

- En este ejemplo, se demuestra la implementación de la POO en JavaScript a través de la creación de una clase Libro que encapsula los datos y el comportamiento de los objetos libro. Además, se muestra cómo crear instancias de esta clase y cómo utilizar sus métodos para mostrar la información de los libros en una página web