<template>
  <main>
    <section class="presentation">
      <h1>Hello, I'm User Kbite</h1>
      <p>Aliquam pharetra sit amet eros id egestas. Ut aliquet tellus eget maximus auctor. 
        Aliquam erat volutpat. Fusce quis convallis mi, et condimentum elit. Phasellus finibus, 
        ipsum a commodo facilisis, elit nunc mattis enim, id efficitur risus nisi sit amet purus. 
      </p>
      <a href="#projects" id="project__btn">Projects</a>
      <a href="#footer" id="icon">
        <svg xmlns="http://www.w3.org/2000/svg" x="0px" y="0px"
        width="50" height="50"
        viewBox="0 0 172 172"
        style=" fill:#000000;">
        <g fill="none" fill-rule="nonzero" stroke="none" stroke-width="1" stroke-linecap="butt" stroke-linejoin="miter" stroke-miterlimit="10" stroke-dasharray="" stroke-dashoffset="0" font-family="none" font-weight="none" font-size="none" text-anchor="none" style="mix-blend-mode: normal">
          <path d="M0,172v-172h172v172z" fill="none"></path>
          <g fill="#ffffff">
            <path d="M16.6625,44.3975l-7.2025,7.2025l76.54,76.54l76.54,-76.54l-7.2025,-7.2025l-69.3375,69.3375z"></path></g></g></svg>
      </a>
    </section>

    <section id="projects">
      <h1>Projects!</h1>
      <div id="cards">
        <div class="card">
          <p>550x500</p>
        </div>
        <div class="card">
          <p>550x500</p>
        </div>
        <div class="card">
          <p>550x500</p>
        </div>
        <div class="card">
          <p>550x500</p>
        </div>
        <div class="card">
          <p>550x500</p>
        </div>
        <div class="card">
          <p>550x500</p>
        </div>
      </div>
    </section>

    <section id="about">
      <h1>About</h1>
      <p>Aliquam pharetra sit amet eros id egestas. Ut aliquet tellus eget maximus auctor.
        Aliquam erat volutpat. Fusce quis convallis mi, et condimentum elit.
        Phasellus finibus, ipsum a commodo facilisis, elit nunc mattis enim, id efficitur risus nisi sit amet purus.
        Aliquam erat volutpat. Fusce quis convallis mi, et condimentum elit.
        Phasellus finibus, ipsum a commodo facilisis, elit nunc mattis enim, id efficitur risus nisi sit amet purus.
      </p>
    </section>

    <section id="contact">
      <h1>Contact</h1>
      <span>💬 user-kbite@gmail.com</span>
      <div class="contact__links">
        <a href="#">Discord</a>
        <a href="#">Instagram</a>
        <a href="#">Github</a>
      </div>
    </section>
  </main>
</template>

<style lang="scss" scoped>
main {
  padding: 4rem 4.5rem;
  display: flex;
  flex-direction: column;
  justify-content: center;

  .presentation {
    color: #fff;
    
    h1 {
      font-size: 4rem;
      max-width: 350px;
    }

    p {
      margin: 1.5rem 0 2rem;
      max-width: 600px;
      font-size: 1.3rem;
      line-height: 1.8rem;
      color: #8b8b8b;
    }

    #project__btn {
      display: none;
      background-color: #fff;
      border-radius: 0.2rem;
      padding: 0.5rem 1rem;
      text-decoration: none;
      color: #000;
      font-size: 1.1rem;
      font-weight: 500;
    }

    #icon {
      display: flex;
      justify-content: center;
      margin-top: 7rem;
    }
  }

  #projects {
    margin-top: 10rem;
    color: #fff;

    h1 {
      text-align: center;
      font-size: 2rem;
    }

    #cards {
      margin-top: 4rem;
      display: flex;
      justify-content: center;
      align-items: center;
      flex-wrap: wrap;

      .card {
        display: flex;
        justify-content: center;
        align-items: center;
        padding-bottom: 1rem;
        width: 550px;
        height: 500px;
        background-color: rgb(14, 13, 13);
        margin: 0 2rem 4rem;
        border-radius: 0.5rem;

        &:hover {
          opacity: 0.5;
          transition-duration: 0.2s;
        }
      }
    }
  }

  #about {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    margin-top: 6rem;
    color: #fff;
    text-align: center;

    h1 {
      font-size: 2rem;
    }

    p {
      margin-top: 2rem;
      max-width: 600px;
      font-size: 1.3rem;
      line-height: 1.8rem;
      color: #8b8b8b;
    }
  } 

  #contact {
    margin-top: 6rem;
    color: #fff;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    text-align: center;

    h1 {
      font-size: 2rem;
    }

    span {
      margin: 3rem 0 2rem;
      background-color: rgb(26, 25, 25);
      padding: 0.9rem 1.2rem 1.2rem;
      border-radius: 1rem;
      font-size: 1.2rem;

      &:hover {
        opacity: 0.9;
        transition-duration: 0.3s;
      }
    }

    .contact__links {
      display: flex;
      justify-content: center;
      flex-wrap: wrap;

      a {
        opacity: 0.5;
        text-decoration: none;
        color: #fff;
        margin: 0 1rem 1.5rem;
        background-color: rgb(36, 36, 36);
        font-size: 1.1rem;
        padding: 0.8rem 1.2rem;
        border-radius: 0.2rem;

        &:hover {
          opacity: 1;
          transition-duration: 0.3s;
        }
      }
    }
  }
}

@media (max-width: 909px) {
  main {
    padding: 4rem 2rem;

    #project__btn {
      display: inline-block !important;
    }
  }
}
</style>