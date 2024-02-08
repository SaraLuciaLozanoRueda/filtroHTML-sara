# FILTRO HTML

Este archivo tiene como finalidad ser la pagina online de la tienda "CampusShop" en ella encontramos catálogos de ropa como abrigos,pantalones y camisetas.

```
.secundario {
    display: grid;
    grid-template: 100%/20% 30% 50%;
    border: 3px solid black;
    display: flex;
    justify-content: center;
    align-items: center;
    margin: 50px;
}

.laterales {
    border-radius: 20px;
    display: flex;
    justify-content: center;
}

.laterales img {
    height: 100px;
    width: 150px;
    border-radius: 20px;
    opacity: .8;
    margin: 5px;
    border: 1px solid black;
}

.prime {
    margin-left: 30px;
}

.fop {
    border-radius: 20px;
    width: 200px;
    transition: .5s ease-in-out;
    margin-left: 20px;
}
.fop:hover{
    scale: 1.1;
    opacity: 0.5;
}
.descripcion {
    margin-left: 50px;
    width: 1000px;
}

button {
    width: 100px;
    background-color: green;
    letter-spacing: 2px;
    text-transform: uppercase;
}

button:hover {
    background: lightgreen;
}
/*RESPONSIVE*/
@media (max-width:768px) {
    .secundario {
        display: flex;
        flex-direction: column;
        border: 3px solid black;
        justify-content: center;
        align-items: center;
    }

    .fotos {
        display: flex;
        align-items: flex-start;
    }

    .laterales img {
        height: 100px;
        width: 150px;
        border-radius: 20px;
        opacity: .8;
    }

    .laterales {
        border-radius: 20px;
        display: flex;
        align-items: flex-start;
    }

    .prime {
        display: flex;
        align-items: center;
        justify-content: center;
        margin: 0px;
    }

    .fop {
        border-radius: 20px;
        height: 300px;
        width: 200px;
        transition: ease-in-out(.5s)
    }
    .fop:hover{
        scale: 1.1;
        opacity: 0.5;
    }
    .descripcion {
        padding: 15px;
        margin-left: 50px;
        width: 340px;
    }
}
```

en las líneas anteriores  definí el estilo para cada uno de los productos, conecte todos los productos al CSS secundariou. Además, hice uso del grid y el flex para organizar la información. En los responsives jugué con los margin y padding para crear una pagina mas estética.

Use una paleta monocromática para que no se pierda la esencia de los productos, cuando te pones sobre una imagen ella te da un efecto de movimiento.

```

* {
    box-sizing: border-box;
    margin: 0px;
    padding: 0px;
}
.carro{
    display: flex;
    border: 1px solid black;
    justify-content: center;
    margin: 10px;
}
.chiqui{
    margin: 5px;
    border-radius: 20px;
}
body {
    display: grid;
    grid-template-columns: 15% auto;
    margin-right: 10px;
    background-color: #CED4DA;
    
}
p{
    text-align: center;
    font-size: 30px;

}
a {
    text-decoration: none;
    color: black;
}

li {
    list-style: none;
    padding: 5px;
    border: 1px solid black;
    border-radius: 10px;
    margin-bottom: 5px;
    margin-left: 5px;
    margin-right: 5px;
}
li:hover{
    background-color:#DEE2E6;
}

.dash {
    margin: 15px;
    background-color: #E9ECEF;
}

h1 {
    font-size: 50px;
    margin-top: 20px;
    text-align: center;
}
h4 {
    text-align: center;
}
h3{
    text-align: center;
    font-size: 15px;
}
.informacion {
    display:grid;
    grid-template-columns: repeat(4,20%);
    justify-content: space-evenly;
    gap: 30px;
}

.cuadritos {
    border: 1px solid black;
    border-radius: 20px;
    padding: 10px;
    width: 90%;
    justify-content: center;
    align-items: center;
    display: flex;
    flex-direction: column;
}
.cuadritos:hover{
    scale: 1.1;
    opacity: 0.5;
}
img {
    width: 80px;
    height: 80px;
    border-radius: 10px;
    margin: 50px;
    margin-top: 5px;
}
button{
    background-color: green;
    color: black;
}
/*RESPONSIVE*/
@media screen and ( max-width:768px) {
    * {
        box-sizing: border-box;
        margin: 0px;
        padding: 0px;
    }
    
    body {
        display: grid;
        grid-template-columns: 15% auto;
        margin-right: 10px;
        background-color: #CED4DA;
    }
    p{
        text-align: right;
        font-size: 20px;
    }
    a {
        text-decoration: none;
        color: black;
    }
    li {
        list-style: none;
        padding: 5px;
        border: 1px solid black;
        border-radius: 10px;
        margin-bottom: 5px;
        margin-left: 5px;
        margin-right: 5px;
    }
    li:hover{
        background-color:#DEE2E6;
    }
    
    .dash {
        margin: 15px;
        background-color: #E9ECEF;
        width: 250%;
    }
    
    h1 {
        font-size: 40px;
        margin-top: 20px;
        text-align: right;
    }
    h4 {
        text-align: center;
    }
    h3{
        text-align:center;
    }

    .informacion {
        display:grid;
        grid-template:repeat(6,20%)/50%;
        justify-content: space-evenly;
        gap: 30px;
        margin-left:100px ;
        
    }
    .cuadritos {
        border: 1px solid black;
        border-radius: 20px;
        padding: 10px; 
        width: 100%;
        justify-content: center;
        align-items: center;
    }
    .cuadritos:hover{
        scale: 1.1;
        opacity: 0.5;
    }
    img {
        width: 150px;
        height: 150px;
        border-radius: 30px;
        margin: 50px;
    }
    .carro{
        display: grid;
        border: 1px solid black;
        justify-content: center;
        margin-left: 150px;
        width: 60%;
        padding:5px;
    }
    .chiqui{
        margin: 5px;
        border-radius: 20px;
    }
}
@media screen and (max-width:500px){
    * {
        box-sizing: border-box;
        margin: 0px;
        padding: 0px;
    }
    
    body {
        display: grid;
        grid-template-columns: 15% auto;
        margin-right: 10px;
        background-color: #CED4DA;
        
    }
    
    a {
        text-decoration: none;
        color: black;
    }
    li {
        list-style: none;
        border: 1px solid black;
        border-radius: 10px;
        margin-bottom: 5px;
        margin-left: 5px;
        margin-right: 5px;
    }
    li:hover{
        background-color:#DEE2E6;
    }
    
    .dash {
        margin: 15px;
        background-color: #E9ECEF;
        width: 250%;
    }
    
    h1 {
        font-size: 30px;
        margin-top: 20px;
        text-align: right;
    }
    h4 {
        text-align: center;
    }
    h3{
        text-align:center;
    }
    .informacion {
        display:grid;
        grid-template:repeat(6,20%)/50%;
        justify-content: space-evenly;
        gap: 30px;
        margin-left:80px ;
        
    }
    .cuadritos {
        border: 1px solid black;
        border-radius: 20px;
        padding: 10px; 
        width: 140%;
        justify-content: center;
        align-items: center;
    }
    .cuadritos:hover{
        scale: 1.1;
        opacity: 0.5;
    }
    img {
        width: 100px;
        height: 100px;
        border-radius: 30px;
        margin: 50px;
    }
    p{
        text-align: right;
        font-size: 15px;
    }

}
```

Este es el CSS que use para la pagina principal. 

En este código use un redireccionamiento para navegar entre las diferentes categorías y tener una  descripción de cada producto. Además use algunos arreglos para la letra, su tamaño,forma y posicionamiento y para la gran mayoría de bordes e imágenes use un border-radius para restar un poco  su figura cuadriculada, un width para darle un tamaño a cada section,div y a los links del dash le quite su decoración para que se vea mas bonio.

