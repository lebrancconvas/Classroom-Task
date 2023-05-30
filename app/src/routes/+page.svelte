<script lang="ts">
  function click() {
    console.log('Sign in with Google...');
  }
</script>

<svelte:head>
  <title>ClearTask | Task Management for Classroom</title>
</svelte:head>

<main>
  <header>
    <div>
      <h1>ClearTask</h1>
    </div>
    <div>
      <h2>Productivity Tool to manage your task</h2>
    </div>
  </header>
  <section id="action">
    <button on:click={click}>
      <img class="google-logo" src="/img/google.png" alt="google-logo"> Login with Google Account
    </button>
  </section>
  <section id="class">
    <div>
      <p>Waiting for Content.....</p>
    </div>
  </section>
</main>

<style>
  * {
    font-family: 'Mulish', sans-serif;
  }


  header {
    text-align: center;
  }

  #action {
    text-align: center;
  }

  button {
    background-color: rgb(56, 188, 249);
    border: none;
    border-radius: 5px;
    color: white;
    cursor: pointer;
    font-size: 26px;
    padding: 10px;
    width: 30%;
    margin: 0 auto;
    max-width: 500px;
  }

  button:hover {
    background-color: #0966ad;
  }

  .google-logo {
    width: 30px;
    height: 30px;
  }

  #class {
    text-align: center;
  }
</style>
