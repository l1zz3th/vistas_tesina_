<script>
</script>

<template>
  <nav class="navbar navbar-expand-lg navbar-light bg-light fixed-top">
    <a class="navbar-brand">Iniciar Sesion</a>
    <button class="navbar-toggler" href="./views/Login/login.vue" data-target="#my-nav" data-toggle="collapse" aria-controls="my-nav" aria-expanded="false" aria-label="Toggle navigation">
      <span class="navbar-toggler-icon"></span>
    </button>
    <div id="my-nav" class="collapse navbar-collapse">
      <ul class="navbar-nav mr-auto">
        <li class="nav-item active">
          <a class="nav-link" href="./views/Login/login.vue">Iniciar Sesion <span class="sr-only">(current)</span></a>
        </li>
        <li class="nav-item">
          <a class="nav-link disabled" href="#" tabindex="-1" aria-disabled="true">Item 2</a>
        </li>
      </ul>
    </div>
  </nav>
</template>

<style>
body{
  background: white;
}

button .navbar-toggler{
  background: orange;

}
</style>