<template>
  <header>
    <h1>CV-WebApp</h1>
    <nav>
      <div id="nav">
        <router-link to="/">Quem sou eu?</router-link> |
        <router-link to="/about">O que faço?</router-link> |
        <router-link to="/hobbie">Hobbies</router-link>
      </div>
    </nav>
  </header>
  <div class="container">
    <router-view />
  </div>
  <footer>
    <div class="footer-links">
      <ul>
        <li>
          <a target="_blank" href="https://www.facebook.com/salomaopena/"
            >Facebook</a
          >
        </li>
        <li>
          <a
            target="_blank"
            href="https://www.linkedin.com/in/salom%C3%A3o-pena-81a7ab177/"
            >Linkedin</a
          >
        </li>
        <li>
          <a target="_blank" href="mailto:spenna.live@gmail.com">Google+</a>
        </li>
        <li>
          <a target="_blank" href="https://www.twitter.com/@pena_salomao">
            Twitter</a
          >
        </li>
      </ul>

      <div class="copyright">
        Copyright &copy; {{ year }} | Designed by
        <a
          target="_blank"
          href="https://www.linkedin.com/in/salom%C3%A3o-pena-81a7ab177/"
          >Salomao Pena</a
        >
      </div>
    </div>
  </footer>
</template>

<style>
#app {
  box-sizing: border-box;
  font-family: Arial, Helvetica, sans-serif;
  margin: auto;
  padding: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
body,
h1,
h2,
h3,
h4,
h5,
h6 {
  font-family: "Lato", sans-serif;
}

body,
html {
  height: 100%;
  color: #777;
  /*color: #141414;*/
  line-height: 1.8;
  background-color: #fbfbfd;
  margin: 0;
}

#nav {
  padding: 30px;
  background-color: #141414;
}

#nav a {
  font-weight: bold;
  color: #fbfbfd;
  text-decoration: none;
}

#nav a:hover {
  color: #d3d3d3;
}

header {
  display: flex;
  border-bottom: 1px solid #ccc;
  padding: 0.5rem 1rem;
  background: #141414;
  font-size: 100%;
  line-height: normal;
  color: #fbfbfd;
}
header h1 {
  margin-left: 1rem;
}

header img {
  height: auto;
  width: 5%;
}

nav {
  margin-left: auto;
}
nav ul {
  list-style: none;
}

nav ul li {
  display: inline-flex;
  margin-left: 1rem;
  margin-top: 10px;
}

.container{
  height:100%;
  padding:5px;
}

footer {
  padding: 0.5rem 1rem;
  background: #141414;
  font-size: 100%;
  line-height: normal;
  color: #fbfbfd;
  text-align: left;
}

.footer-links ul {
  list-style: none;
}

.footer-links ul li {
  display: inline-flex;
  margin-left: 1rem;
  text-align: center;
}

.footer-links ul li a {
  text-decoration: none;
  color: #fbfbfd;
}
.copyright {
  text-align: center;
}
.copyright a {
  text-decoration: none;
  color: #fbfbfd;
}
</style>
