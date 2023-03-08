<script>
  //Variables
  let titulo = " ";
  let subtitulo = "";
  let texto = " ";

  //Funciones del titulo
  function tituloRed() {
    document.getElementById("Title1").style.color = "red";
  }
  function tituloGreen() {
    document.getElementById("Title1").style.color = "green";
  }
  function tituloblue() {
    document.getElementById("Title1").style.color = "blue";
  }

  //Funciones para el subtitulo
  function subtitulored() {
    document.getElementById("Subtitle2").style.color = "red";
  }
  function subtitulogreen() {
    document.getElementById("Subtitle2").style.color = "green";
  }
  function subtituloblue() {
    document.getElementById("Subtitle2").style.color = "blue";
  }

  //Funciones para el texto
  function textored() {
    document.getElementById("Texto2").style.color = "red";
  }
  function textogreen() {
    document.getElementById("Texto2").style.color = "green";
  }
  function textoblue() {
    document.getElementById("Texto2").style.color = "blue";
  }
</script>

<title>Creador de textos Svelte</title>

<h2>Creador de textos</h2>

<!--Aquí es donde el usuario pondra el texto-->
<input bind:value={titulo} placeholder="Titulo" />
<input bind:value={subtitulo} placeholder="subtitulo" />
<input bind:value={texto} placeholder="texto" />

<h4>Opciones de titulo</h4>
<!--Para cambiar el color del titulo-->
<button on:click={tituloRed}>Cambiar el titulo a rojo</button>
<button on:click={tituloGreen}> cambiar el titulo a verde</button>
<button on:click={tituloblue}>cambiar el titulo a azul</button>

<h4>Opciones de subtitulo</h4>
<!--Cambiar el color del subtitulo-->
<button on:click={subtitulored}>Cambiar el subtitulo a rojo</button>
<button on:click={subtitulogreen}>cambiar el subtitulo a verde</button>
<button on:click={subtituloblue}>cambiar el subtitulo a azul</button>

<h4>Opciones de texto</h4>
<!--cambiar el color del texto-->
<button on:click={textored}>cambiar el texto a rojo</button>
<button on:click={textogreen}>cambiar el texto a verde</button>
<button on:click={textoblue}>cambiar el texto a azul</button>

<h1 id="Title1">{titulo}</h1>
<h3 id="Subtitle2">{subtitulo}</h3>
<p id="Texto2">{texto}</p>
