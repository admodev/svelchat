<script>
  export let name;
</script>

<style>
  main {
    text-align: center;
    padding: 1em;
    max-width: 240px;
    margin: 0 auto;
  }

  h1 {
    color: #ff3e00;
    text-transform: uppercase;
    font-size: 4em;
    font-weight: 100;
  }

  p {
    margin-top: 15%;
  }

  .column {
    display: flex;
    flex-direction: column;
    max-width: 80%;
    align-items: center;
    justify-content: center;
    margin-left: auto;
    margin-right: auto;
  }

  button#btnIngresar {
    background-color: orange;
    font-weight: bold;
    border-radius: 10px;
    padding: 10px 25px;
    color: white;
    font-weight: bold;
    text-transform: uppercase;
  }

  @media (min-width: 640px) {
    main {
      max-width: none;
    }
  }
</style>

<main>
  <h1>Bienvenido/a {name}!</h1>
  <p>Por favor inicia sesión para continuar al chat.</p>
  <form method="post">
    <div class="column">
      <input type="text" placeholder="Usuario" />
      <input type="password" placeholder="Contraseña" />
      <button type="submit" id="btnIngresar">Ingresar</button>
    </div>
  </form>
</main>
