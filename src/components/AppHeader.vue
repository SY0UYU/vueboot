<template>
  <nav class="navbar navbar-expand-md navbar-light bg-light">
    <a class="navbar-brand py-0" href="#"></a>
    <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarContent" aria-controls="navbarContent" aria-expanded="false" aria-label="Toggle navigation">
      <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse" id="navbarContent">
      <ul class="navbar-nav mr-auto">
        <li class="nav-item active">
          <a class="nav-link" href="#">Home <span class="sr-only">(current)</span></a>
        </li>
        <li class="nav-item">
          <a class="nav-link" target="_blank" :href="myGithub">Github</a>
        </li>
        <li class="nav-item dropdown">
          <a class="nav-link dropdown-toggle" href="#" id="navbarDropdown" role="button" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
            更加了解我
          </a>
          <div class="dropdown-menu" aria-labelledby="navbarDropdown">
            <a class="dropdown-item" :href="myBlog">My blog</a>
            <a class="dropdown-item" :href="mySteam">My steam</a>
            <div class="dropdown-divider"></div>
            <a class="dropdown-item" href="#">如果你还想更加</a>
            <a class="dropdown-item" href="#">了解我，欢迎邮</a>
            <a class="dropdown-item" href="#">箱联系我</a>
          </div>
        </li>
      </ul>
      <form class="form-inline my-2 my-lg-0">
        <input class="form-control mr-sm-2" type="search" placeholder="Search" aria-label="Search">
        <button class="btn btn-outline-success my-2 my-sm-0" type="submit">Search</button>
      </form>
      <ul class="navbar-nav ml-sm-0 ml-md-3">
        <li class="navbar-item"><a class="nav-link" href="#">登录</a></li>
        <li class="navbar-item"><a class="nav-link" href="#">注册</a></li>
      </ul>
    </div>
  </nav>
</template>

<script>
export default {
  name: 'AppHeader',
  data () {
    return {
      myGithub: 'https://github.com/SY0UYU',
      myBlog: '#',
      mySteam: '#',
      searchText: 'https://www.baidu.com/s?wd=baidu'
    }
  },
  mount () {},
  method () {},
  compute () {}
}
</script>

<style scoped>
.navbar-brand {
  background: url("../assets/img/logo1.png") center center;
  background-size: cover;
  width: 40px;
  height: 40px;
}
</style>
