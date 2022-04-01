<template>
  <nav class="navbar navbar-expand-lg navbar-light">
    <div class="container">
      <a class="navbar-brand" href="#"
        ><img :src="logo" alt="" class="d-inline-block align-text-top my-0"
      /></a>
      <button
        class="navbar-toggler"
        type="button"
        data-bs-toggle="collapse"
        data-bs-target="#navbarSupportedContent"
      >
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarSupportedContent">
        <form class="d-flex ms-auto" id="search">
          <input
            type="search"
            class="form-control"
            placeholder="Search"
            :style="{ backgroundImage: `url(${search})` }"
          />
        </form>
        <ul class="navbar-nav ms-auto mb-2 mb-lg-0">
          <li class="nav-item">
            <a class="nav-link active" href="#">
              <img :src="home" alt="" class="d-inlike-block" />
            </a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">
              <img :src="direct" alt="" class="d-inlike-block" />
            </a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">
              <img :src="new_post" alt="" class="d-inlike-block" />
            </a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">
              <img :src="discover" alt="" class="d-inlike-block" />
            </a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">
              <img :src="liked" alt="" class="d-inlike-block" />
            </a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">
              <div id="avatar-wrap">
                <img :src="avatar" alt="" id="avatar" />
              </div>
            </a>
          </li>
        </ul>
      </div>
    </div>
  </nav>
</template>

<style scoped>
.navbar-brand {
  padding-top: 0 !important;
  padding-bottom: 0 !important;
}

.navbar-brand img {
  height: 38px;
  mix-blend-mode: luminosity;
}

.navbar {
  background-color: white;
  border-bottom: 1px solid #e5e5e5;
}

#avatar {
  width: 23px;
  height: 23px;
  border-radius: 50%;
}

#avatar-wrap {
  border: 1px solid black;
  border-radius: 50%;
  padding: 1px;
  width: 100%;
  height: 100%;
  display: flex;
  justify-content: center;
  align-items: center;
}

.nav-item:nth-last-child(n + 2) {
  margin-right: 0.5rem;
}

#search > input {
  background-repeat: no-repeat;
  background-position: 15px center;
  padding-left: 40px;
}
</style>

<script setup>
import logo from "../assets/logo-dark.png";
import home from "../assets/icons/home.svg";
import liked from "../assets/icons/liked.svg";
import discover from "../assets/icons/discover.svg";
import new_post from "../assets/icons/new.svg";
import avatar from "../assets/avatar.jpg";
import direct from "../assets/icons/direct.svg";
import search from "../assets/icons/search.svg";
</script>
