<template>
  <nav class="navbar navbar-expand-md navbar-light bg-light px-md-5 shadow">
    <a class="navbar-brand pt-0 pb-0" href="#"></a>
    <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
      <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse" id="navbarSupportedContent">
      <ul class="navbar-nav mr-md-auto">
        <li class="nav-item active">
          <a class="nav-link" href="#">Home <span class="sr-only">(current)</span></a>
        </li>
        <li class="nav-item">
          <a class="nav-link" target="_blank" :href="myGithub">Github</a>
        </li>
        <li class="nav-item dropdown">
          <a class="nav-link dropdown-toggle" href="#" id="navbarDropdown" role="button" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
            myOtherWebSite
          </a>
          <div class="dropdown-menu" aria-labelledby="navbarDropdown">
            <a class="dropdown-item" href="#">Action</a>
            <a class="dropdown-item" href="#">Another action</a>
            <div class="dropdown-divider"></div>
            <a class="dropdown-item" href="#">Something else here</a>
          </div>
        </li>
      </ul>
      <div class="navbar-msg mx-auto">Welcome to my website!</div>
      <form class="form-inline my-2 my-lg-0">
        <input class="form-control mr-sm-2" type="search" placeholder="Search" aria-label="Search">
        <button class="btn btn-outline-success my-2 my-sm-0" type="submit">Search</button>
      </form>
    </div>
  </nav>
</template>

<script>
export default {
  name: 'AppHeader',
  data () {
    return {
      myGithub: 'https://github.com/SY0UYU',
      searchText: 'https://www.baidu.com/s?wd=baidu'
    }
  }
}
</script>

<style scoped>
.navbar-brand {
  background: url("../assets/img/logo.png") center center;
  background-size: cover;
  width: 40px;
  height: 40px;
}
.shadow {
  box-shadow: 0 .1rem .8rem rgba(0,0,0,.15)!important;
}
@media (min-width: 925px) {
  .navbar-msg{
    display: none;
  }
}
</style>
