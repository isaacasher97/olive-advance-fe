<template>
  <div id="nav-container">
    <nav style="background-color: #183b54" class="navbar navbar-expand-lg">
      <div class="container-fluid">
        <a class="navbar-brand" href="/">
          <img
            style="width: 150px"
            src="/src/assets/Color logo - no background.svg"
          />
        </a>
        <button
          class="navbar-toggler"
          type="button"
          data-bs-toggle="collapse"
          data-bs-target="#navbarNavDropdown"
          aria-controls="navbarNavDropdown"
          aria-expanded="false"
          aria-label="Toggle navigation"
        >
          <div class="icon-toggler">
            <span class="navbar-toggler-icon"></span>
            <span class="navbar-toggler-icon"></span>
            <span class="navbar-toggler-icon"></span>
          </div>
        </button>
        <div class="collapse navbar-collapse" id="navbarNavDropdown">
          <ul class="navbar-nav">
            <li class="nav-item">
              <a class="nav-link" aria-current="page" href="/">Home</a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="/about">About Us</a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="/contact">Contact Us</a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#">APPLY NOW</a>
            </li>
          </ul>
        </div>
      </div>
    </nav>
  </div>
</template>

<script>
export default {
  name: "Navbar",
};
</script>

<style scoped>
.navbar-collapse {
  flex-grow: 0;
}

a {
  color: #f7f7f7;
  font-weight: 800;
}

.navbar-toggler {
  border: none !important; /* Remove border to create the hamburger effect */
  background: transparent; /* Set background to transparent */
  outline: none; /* Remove outline on click */
}

.navbar-toggler-icon {
  background-color: #fff; /* Set hamburger color */
  width: 30px; /* Set width of each line */
  height: 3px; /* Set height of each line */
  margin-bottom: 5px; /* Adjust spacing between lines */
}
.icon-toggler {
  display: flex;
  flex-direction: column;
}
@media screen and (min-width: 1000px) {
  .navbar-nav {
    gap: 50px;
  }
}
</style>
