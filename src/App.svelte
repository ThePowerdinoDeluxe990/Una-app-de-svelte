<script>
  //Variables
  let titulo = " ";
  let subtitulo = "";
  let texto = " ";

  function info() {
    alert("Hecho por ThePowerdinoDeluxe990");
  }

  //Funciones del titulo

  function tituloblack() {
    document.getElementById("Title1").style.color = "black";
  }
  function tituloRed() {
    document.getElementById("Title1").style.color = "red";
  }
  function tituloGreen() {
    document.getElementById("Title1").style.color = "lightgreen";
  }
  function tituloblue() {
    document.getElementById("Title1").style.color = "blue";
  }

  //Funciones para el subtitulo
  function subtituloblack() {
    document.getElementById("Subtitle2").style.color = "black";
  }

  function subtitulored() {
    document.getElementById("Subtitle2").style.color = "red";
  }
  function subtitulogreen() {
    document.getElementById("Subtitle2").style.color = "lightgreen";
  }
  function subtituloblue() {
    document.getElementById("Subtitle2").style.color = "blue";
  }

  //Funciones para el texto
  function textoblack() {
    document.getElementById("Texto2").style.color = "black";
  }
  function textored() {
    document.getElementById("Texto2").style.color = "red";
  }
  function textogreen() {
    document.getElementById("Texto2").style.color = "lightgreen";
  }
  function textoblue() {
    document.getElementById("Texto2").style.color = "blue";
  }
</script>

<div id="box" />

<title>Creador de textos Svelte</title>

<h2>Creador de textos</h2>

<!--Aquí es donde el usuario pondra el texto-->
<input bind:value={titulo} placeholder="Titulo" />
<input bind:value={subtitulo} placeholder="subtitulo" />
<input bind:value={texto} placeholder="texto" />

<h4>Opciones de titulo</h4>
<!--Para cambiar el color del titulo-->
<button on:click={tituloblack}>Cambiar el titulo a negro</button>
<button on:click={tituloRed}>Cambiar el titulo a rojo</button>
<button on:click={tituloGreen}> cambiar el titulo a verde</button>
<button on:click={tituloblue}>cambiar el titulo a azul</button>

<h4>Opciones de subtitulo</h4>
<!--Cambiar el color del subtitulo-->
<button on:click={subtituloblack}>Cambiar el subtitulo a negro</button>
<button on:click={subtitulored}>Cambiar el subtitulo a rojo</button>
<button on:click={subtitulogreen}>cambiar el subtitulo a verde</button>
<button on:click={subtituloblue}>cambiar el subtitulo a azul</button>

<h4>Opciones de texto</h4>
<!--cambiar el color del texto-->
<button on:click={textoblack}>cambiar el texto a negro</button>
<button on:click={textored}>cambiar el texto a rojo</button>
<button on:click={textogreen}>cambiar el texto a verde</button>
<button on:click={textoblue}>cambiar el texto a azul</button>

<h1 id="Title1">{titulo}</h1>
<h3 id="Subtitle2">{subtitulo}</h3>
<p id="Texto2">{texto}</p>

<button on:click={info}>Creditos</button>

<style>
  #box {
    background-color: white;
    width: 650px;
    height: 650px;
    color: grey;
    position: absolute;
    padding-top: 0px;
    padding-left: 140px;
    left: 300px;
    border-width: 15px;
    border-color: lightblue;
    border-style: ridge;
    box-shadow: 20px 20px 10px;
  }
  button {
    font-family: "Segoe UI", Tahoma, Geneva, Verdana, sans-serif;
    position: relative;
    text-align: center;
    left: 330px;
    box-shadow: 2px 5px 10px;
  }
  input {
    position: relative;
    left: 330px;
    box-shadow: 10px 10px 17px;
  }
  h1 {
    font-family: Arial, Helvetica, sans-serif;
    position: relative;
    left: 330px;
  }
  h3 {
    position: relative;
    left: 330px;
    font-family: Arial, Helvetica, sans-serif;
  }
  p {
    position: relative;
    left: 330px;
    font-family: Arial, Helvetica, sans-serif;
  }
  h4 {
    position: relative;
    left: 330px;
    font-family: Impact, Haettenschweiler, "Arial Narrow Bold", sans-serif;

    color: dark;
  }
  h2 {
    position: relative;
    left: 330px;
    padding-top: 20px;
    font-family: Impact, Haettenschweiler, "Arial Narrow Bold", sans-serif;
    color: dark;
  }
</style>
