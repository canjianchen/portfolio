<template>
  <div class="home">
    <!-- Main -->
    <nav>
      <!-- Bar Icon -->
      <input type="checkbox" name="" id="check" />
      <label for="check" class="checkbtn">
        <i class="fas fa-bars" id="menu-open" @click="menuOpen()"></i>
        <i class="fas fa-times" @click="hide()" id="menu-close"></i>
      </label>
      <!-- menu -->
      <div class="logo">Portfolio</div>
      <ul class="desktop-menu-bar menu-animation">
        <li>
          <a class="text-decoration-none" href="#about"
            ><span>01. </span>About</a
          >
        </li>
        <li>
          <a class="text-decoration-none" href="#experience"
            ><span>02. </span>Education</a
          >
        </li>
        <li>
          <a class="text-decoration-none" href="#work"><span>03. </span>Project</a>
        </li>
        <li>
          <a class="text-decoration-none" href="#leetcode"
            ><span>04. </span>Leetcode</a
          >
        </li>
        <li>
          <a class="text-decoration-none" href="#contact"
            ><span>05. </span>Contact</a
          >
        </li>
        <li>
          <a
            class="btn resume-btn btn-lg"
            target="_blank"
            href=""
            >Resume</a
          >
        </li>
      </ul>
      <ul class="mobile-menu-bar menu-animation">
        <li>
          <a class="text-decoration-none" href="#about"
            ><span>01. </span> <br />
            About</a
          >
        </li>
        <li>
          <a class="text-decoration-none" href="#experience"
            ><span>02. </span><br />Education</a
          >
        </li>
        <li>
          <a class="text-decoration-none" href="#work"
            ><span>03. </span><br />Project</a
          >
        </li>
        <li>
          <a class="text-decoration-none" href="#leetcode"
            ><span>04. </span><br />Leetcode</a
          >
        </li>
        <li>
          <a class="text-decoration-none" href="#contact"
            ><span>05. </span><br />Contact</a
          >
        </li>
        <li>
          <a class="btn resume-btn btn-lg" target="_blank" href="">Resume</a>
        </li>
      </ul>
    </nav>
  </div>
</template>
<script>
export default {
  data() {
    return {};
  },
  methods: {
    menuOpen() {
      document.getElementById("menu-open").style.display = "none";
      document.querySelector(".fa-times").style.display = "block";
    },
    hide() {
      document.getElementById("menu-close").style.display = "none";
      document.getElementById("menu-open").style.display = "block";
    },
  },
};
</script>
<style scoped>
.fa-times {
  display: none;
}
#menu-open {
  margin-top: 15px;
}
</style>