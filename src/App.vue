<script setup>
import Navbar from "./components/Navbar.vue";
import avatar from "./assets/avatar.jpg";
import settings from "./assets/icons/settings.svg";
import school from "./assets/icons/school.svg";
import saved from "./assets/icons/saved.svg";
import posts from "./assets/icons/posts.svg";
import post1 from "./assets/post1.png"
import post2 from "./assets/post2.png"
import post3 from "./assets/post3.png"
import post4 from "./assets/post4.png"
import post5 from "./assets/post5.png"

</script>

<template>
  <navbar />
  <div class="container my-4">
    <div class="row mb-4">
      <div class="col-4 d-flex align-items-center justify-content-center">
        <img :src="avatar" alt="" id="avatar-main" />
      </div>
      <div class="col">
        <div class="d-flex flex-row align-items-center mb-1">
          <div id="nickname" class="me-2">alantheknight</div>

          <div class="me-2">
            <div class="btn btn-sm btn-outline-dark">Edit profile</div>
          </div>
          <div>
            <img :src="settings" alt="" />
          </div>
        </div>

        <div class="mb-3">
          <span class="badge bg-warning me-2">Золотой бобёр</span>
          <span class="badge bg-primary me-2">10 "З"</span>
        </div>

        <div class="d-flex flex-row align-items-center mb-3">
          <div class="me-4">
            <span class="fw-bold">5</span>
            posts
          </div>
          <div class="me-4">
            <span class="fw-bold">100</span>
            followers
          </div>
          <div class="me-4">
            <span class="fw-bold">20</span>
            following
          </div>
        </div>

        <div class="fw-bold">Maxim Gusev</div>
        <div>
          <span>Full Stack Developer</span>
          <div class="d-flex align-items-center">
            <img :src="school" height="15" class="me-2" />
            <span>Academic Gymnasium №56, St. Petersburg, Russia</span>
          </div>
        </div>
      </div>
    </div>

    <div class="w-100 mb-2">
      <ul class="nav nav-tabs justify-content-center">
        <li class="nav-item">
          <a class="nav-link active"><img :src="posts" class="me-2" />Posts</a>
        </li>
        <li class="nav-item">
          <span class="nav-link disabled"
            ><img :src="saved" class="me-2" />Saved</span
          >
        </li>
      </ul>
    </div>

    <div class="row gx-4 gy-4 posts">
      <div class="col-4">
        <img :src="post1" class="img-fluid"/>
      </div>
      <div class="col-4">
        <img :src="post2"  class="img-fluid"/>
      </div>
      <div class="col-4">
        <img :src="post3"  class="img-fluid"/>
      </div>
      <div class="col-4">
        <img :src="post4"  class="img-fluid"/>
      </div>
      <div class="col-4">
        <img :src="post5"  class="img-fluid"/>
      </div>
    </div>

  </div>
</template>

<style>
#app {
  font-family: Inter, sans-serif;
}

#avatar-main {
  width: 120px;
  height: 120px;
  border-radius: 50%;
}

#nickname {
  font-size: 1.4rem;
  font-weight: bold;
}

.posts img {
  aspect-ratio: 1/1;
}

.container {
  max-width: 900px !important;
}
</style>
