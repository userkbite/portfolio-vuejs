<template>
  <header>
    <a href="/">user-kbite</a>
    <nav>
      <li><a href="#projects">Projects</a></li>
      <li><a href="#about">About</a></li>
      <li><a href="#contact">Contact</a></li>
    </nav>
  </header>
</template>

<style lang="scss" scoped>
header {
  display: flex;
  padding: 3rem 4.5rem;
  justify-content: space-between;

  a {
    color: #fff;
    text-decoration: none;
    text-transform: uppercase;
    font-weight: 500;
    font-size: 0.9rem;
  }

  nav {
    display: flex;
    li {
      list-style: none;
      
      a {
        margin: 0 0 0 3rem;
      }
    }
  }
}

@media (max-width: 909px) {
  header {
    padding: 2.5rem 2rem;

    nav {
      display: none;
    }
  }
}
</style>