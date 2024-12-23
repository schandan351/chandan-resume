<script setup>
import ResumeHeader from './components/ResumeHeader.vue'
import Summary from './components/Summary.vue'
import Experience from './components/Experience.vue'
import Sidebar from './components/Sidebar.vue'

</script>

<template>
  <div class="resume">
    <div class="main-content">
      <ResumeHeader />
      <Summary />
      <Experience />
    </div>
    <Sidebar />
  </div>
</template>

<style>
.resume {
  display: grid;
  grid-template-columns: 1fr 400px;
  gap: 2rem;
  max-width: 1200px;
  margin: 2rem auto;
  padding: 2rem;
  font-family: Inter, system-ui, sans-serif;
  color: #213547;
  background-color: #ffffff;
}

.main-content {
  padding-right: 2rem;
}

@media (max-width: 1024px) {
  .resume {
    margin: 1rem;
    padding: 1.5rem;
  }
}

@media (max-width: 768px) {
  .resume {
    grid-template-columns: 1fr;
    margin: 0;
    padding: 1rem;
    border-radius: 0;
  }

  .main-content {
    padding-right: 0;
  }
}
</style>