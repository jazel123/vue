<script setup>
import MainLayout from '../components/MainLayout.vue';

// Page Title of Views
const pageTitle = 'Projects'
</script>

<template>
  <MainLayout :pageTitle="pageTitle">
    <section>
        <h1>SKILLS:</h1>
        <br>
        <h2>PROGRAMMING LANGUAGE:</h2>
        <div class="programming">
            <img src="@/assets/html.png" alt="Photo of HTML">
            <img src="@/assets/css.png" alt="Photo of CSS">
            <img src="@/assets/vue.png" alt="Photo of VUE JS">
        </div>
        <br>
        <h2>Instruments</h2>
        <br>
        <br>
        <div class="ins">
            <img src="@/assets/guitar.jpg" alt="Photo of guitar" class="guitar">
            <img src="@/assets/recorder.jpg" alt="Photo of Recorder" class="recorder">
        </div>
        <h2>COOKING</h2>
        <div class="cook">

            <img src="@/assets/p.jpg" alt="food">

            <img src="@/assets/e.jpg" alt="food">

            <img src="@/assets/a.jpg" alt="food">

            <img src="@/assets/b.jpg" alt="food">

        </div>

    </section>
  </MainLayout>
</template>
<style scoped>
.ins, .programming{
    display: inline-flex;
    flex-direction: row;
    align-items: center;
    margin-left: 20%;
    justify-content: space-between;
}
.cook {
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
    margin: 0 auto;
}
h1 {
    color: black;
    font-size: 3rem;
    text-align: center;
      font-family: 'Times New Roman', Times, serif;
}
h2{
    color: black;
    font-size: 2rem;
    text-align: center;
      font-family: 'Times New Roman', Times, serif;
}
.cook img {
    width: 30%;
    margin-bottom: 20px;
}
@media screen and (max-width: 768px) {
    .ins, .programming, .cook {
        flex-direction: column;
        align-items: center;
        margin-left: auto;
        margin-right: auto;
    }
    .cook img {
        width: 80%;
    }
}

</style>
