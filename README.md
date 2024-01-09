let nob = document.getElementById("No")

nob.addEventListener("mousemove", function() {
    let alto = random(1,10)
    let ancho = random(1,10)
    console.log(alto, ancho)
    nob.style.gridRow = alto;
    nob.style.gridColumn = ancho;

    })


function random(min,max) {
    let numero = Math.floor(Math.random() * (max - min + 1) + min)
    return numero
}

let sib = document.getElementById("Si")

sib.addEventListener("click", function() {
    document.getElementById("p").removeAttribute("hidden")
    console.log("click")
    document.getElementById("1").style.color = "transparent";
    document.getElementById("Si").style.display = "none";
    document.getElementById("No").style.display = "none";
})
div {
    display: flex;
    flex-direction: column;
    align-items: center;
}


h1 {
    padding: 10px;
    color: #711DB0;
}



button {
    color: brown;
    width: 80px;
    height: 40px;
    border: 3px solid #711DB0;
    border-radius: 10px;
    background-color: transparent;
    font-size: xx-large;
    
}

#Si {
    grid-row:  5;
    grid-column: 5;
}

#No {
    grid-row: 5;
    grid-column: 6;
    
}

section {
    display: grid;
    grid-template-columns: 10% 10% 10% 10% 10% 10% 10% 10% 10% 10%;
    grid-template-rows: 10% 10% 10% 10% 10% 10% 10% 10% 10% 10%;
    width: 1200px;
    height: 600px;
    align-items: center;
    justify-items: center;
}

body {
    max-width: 1200px;
    max-height: 673px;
    margin: 0 auto;
    background-image: url(/foto/pngtree-landscapes-wallpaper-images-picture-image_3021437.jpg);
    background-repeat: no-repeat; 
    background-position: center center; 
     background-size: cover;
    
}

p {
    font-size: xx-large;
    justify-content: center;
    color: pink;
}
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Te amo</title>
    
    <link rel="stylesheet" href="me_perdonas.css">
    
    
    <style>
        #No {
    grid-row: 5;
    grid-column: 6;
}
    </style>
</head>
<body>  
        <div>
            <p id="p" hidden>Yo tambien te amo</p>
        <h1 id="1">Me Perdonas</h1>
        <section>
        <button id="Si">Si</button>
        <button id="No">No</button>
    </section>
    </div>
   
    <script src="me_perdonas.js"></script>
</body>
</html>
