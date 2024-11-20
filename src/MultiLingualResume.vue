<template>
  <div class="language-selector">

  </div>

  <Resume resumeId="french-resume">
    <SideBar avatar="./assets/avatar.png">

    </SideBar>
    <Main surname="boxboxjason" name="" title="DevOps Engineer">
    </Main>
  </Resume>

  <Resume resumeId="english-resume">
    <SideBar avatar="./assets/avatar.png">

    </SideBar>
    <Main surname="boxboxjason" name="" title="DevOps Engineer">

    </Main>

  </Resume>

</template>

<script>
import Resume from './components/Resume.vue'
import SideBar from './components/sidebar/SideBar.vue';
import Main from './components/main/Main.vue';

export default {
  name: 'MultiLingualResume',
  components: {
    Resume,
    SideBar,
    Main,
  },
}
</script>

<style>
#resumes {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
