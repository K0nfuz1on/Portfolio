<script setup>
  import { onMounted } from 'vue';

  const observer = new IntersectionObserver(entries => {
    entries.forEach(entry => {
      if (entry.isIntersecting) {
        entry.target.classList.add("show");
      } else {
        entry.target.classList.remove("show");
      }
    })
  })

  onMounted(() => {
    const entries = document.querySelectorAll(".hidden");
    entries.forEach(entry => {
      observer.observe(entry);
    });
  });
</script>

<template>
  <section class="section">
    <div class="hero hidden">
      <h1>Hello,<br> my name is <span style="font-style: italic; color: rgb(240, 23, 23);">K0nfuz1on</span></h1>
      <p>a software/web developer</p>
    </div>
  </section>

  <section class="section">
    
    <div class="stack-container hidden">
      <h1>My skills</h1>
      <div class="stacks">

        <div class="stack">
          <img src="./assets/imgs/vue.png" alt="">
          <p>Vue.js</p>
        </div>

        <div class="stack">
          <img src="./assets/imgs/nuxtLogo.png" alt="">
          <p>Nuxt</p>
        </div>

        <div class="stack">
          <img src="./assets/imgs/jsLogo.png" alt="">
          <p>Javascript</p>
        </div>

        <div class="stack">
          <img src="./assets/imgs/htmlLogo.png" alt="">
          <p>HTML</p>
        </div>

        <div class="stack">
          <img src="./assets/imgs/cssLogo.png" alt="">
          <p>CSS</p>
        </div>

        <div class="stack">
          <img src="./assets/imgs/pythonLogo.png" alt="">
          <p>Python</p>
        </div>

        <div class="stack">
          <img src="./assets/imgs/cppLogo.png" alt="">
          <p>C++</p>
        </div>

        <div class="stack">
          <img src="./assets/imgs/Typescript.png" alt="">
          <p>Typescript</p>
        </div>

        <div class="stack">
          <img src="./assets/imgs/firebaseLogo.png" alt="">
          <p>Firebase</p>
        </div>

        <div class="stack">
          <img src="./assets/imgs/gitLogo.png" alt="">
          <p>GIT</p>
        </div>

        <div class="stack">
          <img src="./assets/imgs/sassLogo.png" alt="">
          <p>sass</p>
        </div>

        <div class="stack">
          <img src="./assets/imgs/npmLogo.png" alt="">
          <p>NPM</p>
        </div>

        <div class="stack">
          <img src="./assets/imgs/phpLogo.png" alt="">
          <p>PHP</p>
        </div>

        <div class="stack">
          <img src="./assets/imgs/viteLogo.png" alt="">
          <p>Vite</p>
        </div>

        <!--<div class="stack">
          <img src="./assets/imgs/laravelLogo.png" alt="">
          <p>Laravel</p>
        </div>-->

        <div class="stack">
          <img src="./assets/imgs/mongoDBLogo.png" alt="">
          <p>MongoDB</p>
        </div>

        <div class="stack">
          <img src="./assets/imgs/nodeJS.png" alt="">
          <p>Node.js</p>
        </div>

        <div class="stack">
          <img src="./assets/imgs/expressJSlogo.png" alt="">
          <p>Express.js</p>
        </div>
        
  
      </div>
    </div>
  </section>

  <section class="section">


    <div class="projects-container hidden">
      
        <h1>My Projects</h1>
        <div class="projects">

          <div class="project">
            <img src="./assets/imgs/gameShop.png" alt="">
            <h1>Game Shop website</h1>
            <p>A game shop website that utilizes the RAWG api and lets you add games to cart, built with vue.js, axios, vite with node.js and Express.js as the backend.</p>
          </div>

          <!--<div class="project">
            <img src="" alt="">
            <h1>Event organization app</h1>
            <p>A event organization website built with vue.js, vite, laravel as the backend and mongoDB as the database.</p>
          </div>-->


          <div class="project">
            <img src="./assets/imgs/expenseTracker.png" alt="">
            <h1>Expense Tracker</h1>
            <p>A expense tracker built with vue.js, vite and firebase.</p>
          </div>

          <div class="project">
            <img src="./assets/imgs/taskmanagerPython.png" alt="">
            <h1>Cli ToDo list</h1>
            <p>A command-line ToDo list made with python using the cmd, json and os modules.</p>
            <div class="background-cover"></div>
          </div>

          <div class="project">
            <img src="./assets/imgs/notesApp.png" alt="">
            <h1>CRUD Note taking application</h1>
            <p>A note taking application where you can take create, update and delete notes.</p>
            <div class="background-cover"></div>
          </div>

          <div class="project">
            <img src="./assets/imgs/2dGame.png" alt="">
            <h1>A 2d game against a bot</h1>
            <p>A 2d game where you can fight against a bot while using many different characters, built with vue.js and vite.</p>
            <div class="background-cover"></div>
          </div>

          <div class="project">
            <img src="./assets/imgs/jsMatchCards.png" alt="">
            <h1>JS match cards</h1>
            <p>A match cards game built with pure javascript.</p>
            <div class="background-cover"></div>
          </div>

          <div class="project">
            <img src="./assets/imgs/flashCards.png" alt="">
            <h1>Flash cards learning app</h1>
            <p>A flash cards learning app built with vue.js, vite and firebase.</p>
            <div class="background-cover"></div>
          </div>

          <div class="project">
            <img src="./assets/imgs/vueChat.png" alt="">
            <h1>Real time chat room</h1>
            <p>A real time chat room built with vue.js, vite and agora.</p>
            <div class="background-cover"></div>
          </div>

          


        </div>
    
    </div>
  
  
  </section>

  <section class="section hidden">
    <span>
      <h1 style="text-align: center;">Contact</h1>
      <span>Email: <a style="color: rgb(240, 23, 23);" href="mailto:">K0nfuz1onBussiness@gmail.com</a></span><br>
      <!--<span>GitHub: <a style="color: rgb(240, 23, 23);" href="https://github.com/K0nfuz1on">https://github.com/K0nfuz1on</a></span><br>-->
    </span>
    <span class="copyright">&#169; <mark style="background-color: transparent; color: rgb(240, 23, 23);">K0nfuz1on</mark> 2024</span>
  </section>
    
</template>

<style>
  @import url('https://fonts.googleapis.com/css2?family=Poppins:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&display=swap');

  body {
    background-color: #131316;
    color: white;
    font-family: "poppins", sans-serif;
    margin: 0;
    padding: 0;
  }

  .section {
    display: grid;
    place-items: center;
    align-items: center;
    min-height: 100vh;
  }

  .section:nth-child(1) {
    background-color: #181818;
  }

  .section:nth-child(2) {
    min-height: 110vh;
  }

  .section:nth-child(3) {
    background-color: #161616;
    min-height: 110vh;
  }

  .section:nth-child(4) {
    min-height: 30vh;
    position: relative;
  }
  
  .section:nth-child(4) .copyright  {
    position: absolute;
    bottom: 5px;
  }

  .stack-container {
    text-align: center;
  }

  .stacks {
    display: flex;
    flex-wrap: wrap;
    gap: 15px;
    max-width: 600px;
    justify-content: center;
    align-items: center;
  }

  .stack {
    height: 100px;
    width: 100px;
    border: 1px rgba(0, 0, 0, 0.30) solid;
    display: flex;
    align-items: center;
    justify-content: center;
    border-radius: 12px;
    background-color: #202020;
    flex-direction: column;
    position: relative;
  }

  .stack img {
    width: 60px;
    margin-bottom: 10px;
  }

  .stack p {
    margin: 0;
    position: absolute;
    bottom: 0;
  }

  .projects-container {
    text-align: center;
  }

  .projects {
    display: flex;
    flex-wrap: wrap;
    gap: 30px;
    max-width: 1500px;
    justify-content: center;
    align-items: center;
  }

  .project {
    width: 450px;
    min-height: 250px;
    border: 1px rgba(0, 0, 0, 0.30) solid;
    border-radius: 12px;
    background-color: #202020;
    position: relative;
    transition: all ease 0.5s;
    z-index: 5;
  }

  .project img {
    position: absolute;
    left: 0;
    top: 0;
    width: 75%;
    height: 50%;
    border-top-left-radius: 12px;
    border-bottom-right-radius: 12px;
    background-color: #121212;
  }

  .project h1 {
    position: absolute;
    bottom: 35%;
    left: 2.5%;
    margin: 0;
  }

  .project p {
    position: absolute;
    bottom: 0%;
    height: 30%;
    opacity: 0.8;
    margin: 0;
    left: 2.5%;
  }

  @media only screen and (max-width: 455px) {
    .project {
      width: 400px;
    }
  }

  @media only screen and (max-width: 400px) {
    .project {
      width: 350px;
    }
  }

  @media only screen and (max-width: 300px) {
    .project {
      width: 250px;
    }
  }

  .hidden {
    opacity: 0;
    filter: blur(5px);
    transform: translateX(-100%);
    transition: all 1s;
  }

  .show {
    opacity: 1;
    filter: blur(0);
    transform: translateX(0);
  }
</style>
