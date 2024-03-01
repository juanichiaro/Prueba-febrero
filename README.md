-INICIO 
/HTML
<!DOCTYPE html>
<html lang="es">
<head>
    <title>newells</title>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="author" content="Juan Ignacio Chiarotti"/>
    <meta name="keywords" content="Pc, Computadoras, Celulares,">
    <link rel="stylesheet" href="estilos1.css">
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Nunito&display=swap" rel="stylesheet">
    <link href="https://fonts.googleapis.com/css2?family=Sixtyfour&display=swap" rel="stylesheet">

</head>
<body>
        <div class="header-top">
            <p>NewellsStore</p>
        </div>

        <header class="header">
            <a href="newellsPagina.html" class="ESCRITORIO">INICIO</a>
            <a href="catalogo.html" class="ESCRITORIO1">CATOLOGO</a>
            <a href="Contacto.html" class="ESCRITORIO2">CONTACTO</a>
        </header>

        <div class="Inicio">
            <img src="fondonewells.png"  class="FotoInicio">
        </div>
</body>
</html>

/CSS
body {
    height: 100%; /* Hace que el cuerpo y html ocupen toda la altura de la pantalla */
    background: white;
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    }

a{
    display: inline-block;
    padding: 10px 20px;
    color: black;
    text-decoration: none;
    transition: color 0.3s;
}
.header a:hover {
    color: white;
}

.header-top {
    background-color: black; /* Fondo negro */
    color: white; /* Texto blanco */
    text-align: center; /* Centra el texto horizontalmente */
    font-family: "Sixtyfour", sans-serif;
    padding: 10px 0; /* Espacio arriba y abajo del texto */
}

.header{
   width: 100%; /* Asegura que el header ocupe todo el ancho */
   background-color: red;
   color: black;
   text-align: center; 
   font-family: 'Nunito', sans-serif;  
}

.Inicio {
    width: 100%; /* Asegura que el div ocupe todo el ancho */
}

.FotoInicio {
    width: 100%;
    height: 100%;
    object-fit: cover; /* Asegura que la imagen cubra completamente el div sin perder sus proporciones */
    display: block; /* Elimina cualquier espacio extra alrededor de la imagen */
}

@media only screen and (max-width: 480px) {
    .header {
        height: auto; 
    }
   .Inicio{
         height: auto; 
   }
}




-Catalogo
/HTML
<!DOCTYPE html>
<html lang="es">
<head>
    <title>newells</title>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="author" content="Juan Ignacio Chiarotti"/>
    <meta name="keywords" content="Pc, Computadoras, Celulares,">
    <link rel="stylesheet" href="estilo2.css">
    <script src="script.js"></script>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Nunito&display=swap" rel="stylesheet">
    <link href="https://fonts.googleapis.com/css2?family=Jost:ital,wght@0,100..900;1,100..900&display=swap" rel="stylesheet">
    <link href="https://fonts.googleapis.com/css2?family=Sixtyfour&display=swap" rel="stylesheet">

</head>
<body>


        <div class="header-top">
            <p>NewellsStore</p>
        </div>

        <header class="header">
            <a href="newellsPagina.html" class="ESCRITORIO">INICIO</a>
            <a href="catalogo.html" class="ESCRITORIO1">CATALOGO</a>
            <a href="Contacto.html" class="ESCRITORIO2">CONTACTO</a>
        </header>
        
        <div class="carrusel" id="carrusel">
    <div class="carrusel-items">
        <!-- Item 1 -->
        <div class="item">
            <img src="remera1.jpg" alt="Imagen 1">
            <div class="info">
                <p>Descripción de la imagen 1</p>
                <p>Precio: $10.00</p>
            </div>
        </div>
        <div class="item">
            <img src="remera2.jpg" alt="Imagen 1">
            <div class="info">
                <p>Descripción de la imagen 2</p>
                <p>Precio: $20.00</p>
            </div>
        </div>
        <div class="item">
            <img src="remera3.png" alt="Imagen 1">
            <div class="info">
                <p>Descripción de la imagen 3</p>
                <p>Precio: $30.00</p>
            </div>
        </div>
        <div class="item">
            <img src="remera4.png" alt="Imagen 1">
            <div class="info">
                <p>Descripción de la imagen 4</p>
                <p>Precio: $40.00</p>
            </div>
        </div>
        <div class="item">
            <img src="remera5.png" alt="Imagen 1">
            <div class="info">
                <p>Descripción de la imagen 5</p>
                <p>Precio: $50.00</p>
            </div>
        </div>
        <div class="item">
            <img src="remera6.png" alt="Imagen 1">
            <div class="info">
                <p>Descripción de la imagen 6</p>
                <p>Precio: $60.00</p>
            </div>
        </div>
        <!-- Repite el bloque anterior para cada una de las 6 imágenes, cambiando la ruta de la imagen, la descripción y el precio. -->
    </div>
    <button class="prev" onclick="mover(-1)">&#10094;</button>
    <button class="next" onclick="mover(1)">&#10095;</button>

</div>

<div class="galeria">
    <div class="fila">
        <div class="imagen-container">
            <img src="remera1.jpg" alt="Imagen 1">
            <p>Este código HTML añade un nuevo div justo antes del .header existente, el cual contiene un párrafo .</p>
        </div>
        <div class="imagen-container">
            <img src="remera2.jpg" alt="Imagen 2">
            <p>Este código HTML añade un nuevo div justo antes del .header existente, el cual contiene un párrafo</p>
        </div>
        <div class="imagen-container">
            <img src="remera3.png" alt="Imagen 3">
            <p>Este código HTML añade un nuevo div justo antes del .header existente, el cual contiene un párrafo</p>
        </div>
    </div>
    <div class="fila">
        <div class="imagen-container">
            <img src="remera4.png" alt="Imagen 4">
            <p>Este código HTML añade un nuevo div justo antes del .header existente, el cual contiene un párrafo</p>
        </div>
        <div class="imagen-container">
            <img src="remera5.png" alt="Imagen 5">
            <p>Este código HTML añade un nuevo div justo antes del .header existente, el cual contiene un párrafo</p>
        </div>
        <div class="imagen-container">
            <img src="remera6.png" alt="Imagen 6">
            <p>Este código HTML añade un nuevo div justo antes del .header existente, el cual contiene un párrafo</p>
        </div>
    </div>
</div>
<script src="script.js"></script>
</body>
</html>



/CSS
body {
    background: white;
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    }

a{
    display: inline-block;
    padding: 10px 20px;
    color: black;
    text-decoration: none;
    transition: color 0.3s;
}
.header a:hover {
    color: white;
}

.header-top {
    background-color: black; /* Fondo negro */
    color: white; /* Texto blanco */
    text-align: center; /* Centra el texto horizontalmente */
    font-family: "Sixtyfour", sans-serif;
    padding: 10px 0; /* Espacio arriba y abajo del texto */
}

.header{
   background-color: red;
   color: black;
   text-align: center;
   font-family: 'Nunito', sans-serif;  
}

.carrusel {
    position: relative;
    width: 100%;
    height: 100vh; /* Ocupa el 100% de la altura de la ventana */
    margin: auto;
    overflow: hidden;
}

.carrusel-items .item {
    display: flex;
    flex-direction: column; /* Organiza los elementos hijos verticalmente */
    align-items: center; /* Centra los elementos hijos horizontalmente */
    justify-content: center; /* Centra los elementos hijos verticalmente */
    width: 100%;
    height: 100vh;
    display: none; /* Comienza con todos los ítems ocultos */
}

.carrusel-items img {
    max-width: 80%; /* Ajusta el ancho máximo de la imagen */
    object-fit: contain; /* Asegura que la imagen se ajuste sin distorsionarse */
    margin-bottom: 20px; /* Espacio entre la imagen y el texto debajo */
}

.info {
    text-align: center; /* Centra el texto horizontalmente */
    padding: 0 20px; /* Espacio alrededor del texto */
    font-family: "Jost", sans-serif;
}

.prev, .next {
    cursor: pointer;
    position: absolute;
    top: 50%;
    width: auto;
    padding: 16px;
    margin-top: -22px;
    color: black; /* Color de las flechas */
    font-weight: bold;
    font-size: 18px;
    transition: 0.6s ease;
    user-select: none;
    background-color: rgba(255, 255, 255, 0.5); /* Fondo semi-transparente para mejorar la visibilidad */
}

.prev {
    left: 0;
    border-radius: 0 3px 3px 0;
}

.next {
    right: 0;
    border-radius: 3px 0 0 3px;
}

.info p { /* Estilo para todos los párrafos dentro de .info */
    font-size: 20px; /* Tamaño de fuente general para la descripción y el precio */
}

.info .precio { /* Clase adicional para estilizar específicamente el precio */
    font-size: 24px; /* Tamaño de fuente más grande para el precio */
    font-weight: bold; /* Hace el precio más destacado */
}

.galeria {
    width: 100%;
    margin: auto;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
}

.fila {
    display: flex;
    justify-content: space-around; /* Ajusta esto para cambiar la separación entre imágenes */
    margin-bottom: 20px; /* Espacio entre filas */
}

.imagen-container {
    text-align: center; /* Centra el texto bajo las imágenes */
    flex-basis: 30%; /* Ajusta el ancho de cada imagen y su contenedor de texto */
    border: 2px solid red; /* Añade un borde rojo alrededor de cada contenedor */
    margin: 10px; /* Espacio alrededor de cada contenedor para evitar que los bordes se toquen */
    padding: 10px; /* Espacio interior para separar el contenido del borde */
    box-sizing: border-box; /* Asegura que el padding y el borde se incluyan en el ancho y alto definidos */
}

.imagen-container img {
    width: 100%; /* Hace que la imagen ocupe todo el ancho de .imagen-container */
    height: auto; /* Mantiene la proporción de la imagen */
}

@media only screen and (max-width: 480px) {
    .header {
      height: auto; 
    }
    .header-top{
      height: auto;
    }
    .carrusel{
      height: auto;
    }
    .carrusel-items img{
      height: auto;
    }
    .info{
      height: auto;
    }
    .fila{
      height: auto;
    }
  }




/JS
let indiceActual = 0;

function mostrarItem(indice) {
    const items = document.querySelectorAll('.item');
    if (indice >= items.length) indiceActual = 0;
    if (indice < 0) indiceActual = items.length - 1;
    
    for (let i = 0; i < items.length; i++) {
        items[i].style.display = "none";  
    }
    
    items[indiceActual].style.display = "flex";
}

function mover(n) {
    mostrarItem(indiceActual += n);
}

mostrarItem(indiceActual); // Inicializa el carrusel mostrando el primer ítem




-CONTACTO
/HTML
<!DOCTYPE html>
<html lang="es">
<head>
    <title>newells</title>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="author" content="Juan Ignacio Chiarotti"/>
    <meta name="keywords" content="Pc, Computadoras, Celulares,">
    <link rel="stylesheet" href="estilo3.css">
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Nunito&display=swap" rel="stylesheet">
    <link href="https://fonts.googleapis.com/css2?family=Sixtyfour&display=swap" rel="stylesheet">

</head>
<body>

    <div class="header-top">
        <p>NewellsStore</p>
    </div>

    <header class="header">
        <a href="newellsPagina.html" class="ESCRITORIO">INICIO</a>
        <a href="catalogo.html" class="ESCRITORIO1">CATÁLOGO</a>
        <a href="contacto.html" class="ESCRITORIO2">CONTACTO</a>
    </header>
    <main>
        <form action="https://formspree.io/f/myyqbkkp" method="POST">
            <label for="nombre">Nombre:</label>
            <input type="text" id="nombre" name="nombre" required>

            <label for="email">Correo electrónico:</label>
            <input type="email" id="email" name="_replyto" required>

            <label for="mensaje">Mensaje:</label>
            <textarea id="mensaje" name="mensaje" rows="4" required></textarea>

            <button type="submit">Enviar</button>
        </form>
    </main>
</body>
</html>




/CSS
body {
    height: 100%; /* Hace que el cuerpo y html ocupen toda la altura de la pantalla */
    background: white;
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    }

a{
    display: inline-block;
    padding: 10px 20px;
    color: black;
    text-decoration: none;
    transition: color 0.3s;
}
.header a:hover {
    color: white;
}

.header-top {
    background-color: black; /* Fondo negro */
    color: white; /* Texto blanco */
    text-align: center; /* Centra el texto horizontalmente */
    font-family: "Sixtyfour", sans-serif;
    padding: 10px 0; /* Espacio arriba y abajo del texto */
}

.header{
   width: 100%; /* Asegura que el header ocupe todo el ancho */
   background-color: red;
   color: black;
   text-align: center; 
   font-family: 'Nunito', sans-serif;  
}

main {
    padding: 20px;
}

form {
    max-width: 600px;
    margin: 0 auto;
}

label {
    display: block;
    margin: 10px 0 5px;
}

input[type="text"],
input[type="email"],
textarea {
    width: 100%;
    padding: 10px;
    margin-bottom: 20px;
    border: 1px solid #ccc;
    border-radius: 5px;
}

button {
    background-color: #4CAF50;
    color: white;
    padding: 10px 20px;
    border: none;
    border-radius: 5px;
    cursor: pointer;
}

button:hover {
    background-color: #45a049;
}

@media only screen and (max-width: 480px) {
    .header {
        height: auto; 
    }
    
}




-RESPONSIVE JS
/HTML
<!DOCTYPE html>
<html lang="es">
<head>
    <title>newells</title>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="author" content="Juan Ignacio Chiarotti"/>
    <meta name="keywords" content="Pc, Computadoras, Celulares,">
    <link rel="stylesheet" href="responsive2.css">
    <script src="responsive3.js"></script>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Nunito&display=swap" rel="stylesheet">
    <link href="https://fonts.googleapis.com/css2?family=Sixtyfour&display=swap" rel="stylesheet">
</head>

<body>
<div class="contenedor">
    <div class="imagen izquierda">
        <img src="remera1.jpg" alt="Imagen Izquierda">
    </div>
    <div class="texto">
        <p>Aquí va tu texto en el medio.</p>
    </div>
    <div class="imagen derecha">
        <img src="remera2.jpg" alt="Imagen Derecha">
    </div>
</div>

<script src="responsive3.js"></script>
</body>
</html>





/CSS
.contenedor {
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.imagen img {
    width: 100%;
    height: auto;
}

.imagen.izquierda, .imagen.derecha {
    flex-basis: 20%; /* Ajusta este valor según necesites */
}

.texto {
    flex-basis: 55%; /* Ajusta este valor según necesites */
    text-align: center;
}





/JS
document.addEventListener("DOMContentLoaded", function() {
    var contenedor = document.querySelector('.contenedor');
    var imagenes = document.querySelectorAll('.imagen');
    var texto = document.querySelector('.texto');

    function ajustarDisposicion() {
        if (window.innerWidth <= 768) {
            // Cambia a disposición vertical
            contenedor.style.flexDirection = 'column';
            imagenes.forEach(function(imagen) {
                imagen.style.flexBasis = 'auto';
            });
            texto.style.flexBasis = 'auto';
        } else {
            // Vuelve a la disposición original horizontal
            contenedor.style.flexDirection = 'row';
            imagenes.forEach(function(imagen) {
                imagen.style.flexBasis = '20%'; // Ajusta según necesidad
            });
            texto.style.flexBasis = '55%'; // Ajusta según necesidad
        }
    }

    // Llama a ajustarDisposicion al cargar la página
    ajustarDisposicion();

    // Añade un evento para ajustar la disposición cuando se cambie el tamaño de la ventana
    window.addEventListener('resize', ajustarDisposicion);
});
