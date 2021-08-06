<template>
  <nav
      class="navbar w-100 align-items-center navbar-expand-lg navbar bg-white py-3 nav-trans">
    <div class="container-fluid d-flex px-3 px-md-0">
      <a class="navbar-brand d-flex">
        <img src="../assets/logo.png"
             class="img-fluid logo" alt="">
      </a>
      <div class="" id="navbarText">
        <ul class="navbar-nav ml-auto mr-0 d-flex align-items-lg-center">
          <li class="nav-item">
            <a class="nav-link text-uppercase">About</a>
          </li>
          <li class="nav-item">
            <a class="nav-link text-uppercase">Work</a>
          </li>
          <li class="nav-item">
            <a class="nav-link text-uppercase">Contact</a>
          </li>
          <li class="nav-item">
            <a class="nav-link text-uppercase">Ideas</a>
          </li>
          <li class="nav-item">
            <a class="nav-link text-uppercase"><i class="fa fa-search" aria-hidden="true"></i></a>
          </li>
        </ul>
      </div>
    </div>
  </nav>
</template>

<script>
export default {
  name: 'Navbar',
}
</script>

<style lang="scss">
.container-fluid {
  width: 90% !important;
  @media screen and (min-width: 320px) and (max-width: 991px) {
    width: 100%;
  }
}

.logo {
  max-width: 240px !important;
}

.nav-item {
  a {
    color: #333333;
    font-family: SourceRegular;
    font-size: 20px;
    margin-right: 20px;
    cursor: pointer;
  }

  &:last-child a {
    font-size: 25px;
  }

  .feature-text {
    color: #ffffff;
  }
}

.navbar-nav {
  li.active {
    a {
      color: #50c9bc !important;
    }
  }
}

.nav-change {
  li.active {
    a {
      color: #50c9bc !important;
    }
  }
}

.nav-change {
  .active-change.active {
    a {
      color: #50c9bc !important;
    }
  }
}

@media screen and (min-width: 320px) and (max-width: 991px) {
  .nav-item {
    display: contents !important;
  }
}

.navbar-toggler {
  color: rgba(0, 0, 0, .5);
  border-color: rgba(0, 0, 0, .1);

  &:focus {
    outline: none;
  }
}

.navbar-toggler-icon {
  background-image: url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' width='30' height='30' viewBox='0 0 30 30'%3e%3cpath stroke='rgba(0, 0, 0, 0.5)' stroke-linecap='round' stroke-miterlimit='10' stroke-width='2' d='M4 7h22M4 15h22M4 23h22'/%3e%3c/svg%3e");
}

</style>
