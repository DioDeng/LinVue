<template>
  <section :class="navBarSet">
    <nav class="navbar navbar-expand-lg">
      <div class="container">
        <a class="navbar-brand" href="#">LOGO</a>
        <div>
          <button
            class="navbar-toggler"
            type="button"
            data-bs-toggle="collapse"
            data-bs-target="#navbarSupportedContent"
            aria-controls="navbarSupportedContent"
            aria-expanded="false"
            aria-label="Toggle navigation"
          >
            <span class="navbar-toggler-icon"></span>
          </button>
          <div class="collapse navbar-collapse" id="navbarSupportedContent">
            <ul class="navbar-nav me-auto mb-2 mb-lg-0">
              <li class="nav-item">
                <router-link class="nav-link ms-4 text-light" to="about"
                  >關於我們</router-link
                >
              </li>
              <li class="nav-item">
                <router-link class="nav-link ms-4 text-light" to="service"
                  >服務項目</router-link
                >
              </li>
              <li class="nav-item">
                <router-link class="nav-link ms-4 text-light" to="news"
                  >最新消息</router-link
                >
              </li>
              <li class="nav-item">
                <router-link class="nav-link ms-4 text-light" to="show"
                  >網頁展示</router-link
                >
              </li>
              <li class="nav-item">
                <router-link class="nav-link ms-4 text-light" to="connection"
                  >聯絡我們</router-link
                >
              </li>
            </ul>
          </div>
        </div>
      </div>
    </nav>
  </section>
</template>

<script>
export default {
  data() {
    return {
      navBarSet: '',
    };
  },
  mounted() {
    window.addEventListener('scroll', () => {
      const windowY = window.scrollY;
      const breakpoint = window.innerHeight;
      if (windowY > breakpoint) {
        this.navBarSet = 'bg-dark';
      } else {
        this.navBarSet = '';
      }
    });
  },
};
</script>
