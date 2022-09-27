<script setup>
defineProps({
  text: {

    default: "",

  },
  count: {
    default: 0,
  },
})
</script>


<template>
  <nav class="navbar navbar-expand-lg bg-light">
    <div class="container-fluid">
      <a class="navbar-brand" href="#">Navbar</a>
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent"
              aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarSupportedContent">
        <ul class="navbar-nav me-auto mb-2 mb-lg-0">
          <li class="nav-item">
            <a class="nav-link active" aria-current="page" href="#">Home</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">Link</a>
          </li>
          <li class="nav-item dropdown">
            <a class="nav-link dropdown-toggle" href="#" role="button" data-bs-toggle="dropdown" aria-expanded="false">
              Dropdown
            </a>
            <ul class="dropdown-menu">
              <li><a class="dropdown-item" href="#">Action</a></li>
              <li><a class="dropdown-item" href="#">Another action</a></li>
              <li>
                <hr class="dropdown-divider">
              </li>
              <li><a class="dropdown-item" href="#">Something else here</a></li>
            </ul>
          </li>
          <li class="nav-item">
            <a class="nav-link disabled">Disabled</a>
          </li>
        </ul>
        <form class="d-flex" role="search">
          <input class="form-control me-2 bg-black" type="search" placeholder="Search" aria-label="Search">
          <button class="btn btn-outline-success bg-dark" type="submit">Search</button>
        </form>
      </div>
    </div>
  </nav>
  <div>
    <h1 class="text-center">{{ text }}</h1>
    <input type="text" class="input-group-text bg-dark text-bg-dark" v-model="text">
    <div class="container">

    </div>
  </div>
  <div ><h1 style="margin-left: 122px">{{count}}</h1>
    <button class="btn btn-outline-success bg-dark " @click="count--">WOOPS ! PLUS -</button>
    <button class="btn btn-outline-success bg-dark " @click="count++">WOOPS ! PLUS +</button>

  </div>

</template>


<style scoped>

</style>
