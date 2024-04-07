<script setup>
import MainLayout from '../components/MainLayout.vue';

// Page Title of Views
const pageTitle = 'About'
</script>

<template>
  <MainLayout :pageTitle="pageTitle">
    <body>
      <div class="about">
        <h1>ABOUT ME</h1>
      </div>

    <section class="flex flex-col items-center justify-center">
      <div class="img">
        <img src="@/assets/me.jpg"
             alt="Jazel Pangasi-an"/>
      </div>
      <br>
      <div class="info">
        <h2>Name:</h2>
        <p>Jazel Pangasi-an</p>
        <br>
        <h2>Address:</h2>
        <p>Purok Kamunggay, Brgy. Alegria, Cordova, Cebu</p>
        <br>
        <h2>Birthdate:</h2>
        <p>May 08, 2003</p>
        <br>
        <h2>Age:</h2>
        <p>20</p>
        <br>

        <h2>Hobbies:</h2>
        <ul style="list-style-type:square; margin-left: 10%;">
          <li>Cooking</li>
          <li>Playing Online Games</li>
          <li>Sleeping</li>
        </ul>
        <br>
        <h2>Height:</h2>
        <p>5'4</p>
      </div>
      <br>
      <div class="msg">
        <h1>ALL ABOUT ME</h1>
        <p>I am Jazel Pangasi-an and currently living here in Alegria, Cordova. I am living alone in a small apartment that I rented,  though the money is not my own. I finally have experience living alone, though living alone is not as smooth as what I was expected but this is what I dream. </p>
        <br>
        <p>I grow up in a not complete family, in short a broken family. I have seen my father and mother bickering and fighting. They've just decided to split up, not wanting to hurt each other more. In the Age of 18, I decided to just work instead of going to college because I want to help my father financially but my mother is against it. She decided to send me here in Cebu, where my brother and his wife live. Well, I live there for 2 years and as time goes by, conflicts are there. I decided to live on my own to avoid the conflicts. </p>
        <br>
        <p>Now, I am independent in all ways. I do my chores, wash the dishes, wash my clothes without using machine. I did not regret my decision because this makes me feel free.
        </p>
      </div>

    </section>
    </body>
  </MainLayout>
</template>

<style scoped>
body {

  min-height: 100vh;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}

.info {
  text-align: justify;
}

h1 {
  color: black;
  font-size: 3rem;
  text-align: center;
    font-family: 'Times New Roman', Times, serif;
}

h2 {
  color: black;
  font-size: larger;
  margin-left: 5%;
}

p {
  margin-left: 5%;
}

.img {
  width: 15%;
  text-align: center;
  margin-top: 10px;
}
.img img{
    border-radius: 20px;
}
</style>
