<script setup>
const education = [
  {
    degree: 'Bachelor in Software Engineering',
    school: 'Nepal College of Information Technology (NCIT), Kathmandu, Nepal',
    period: '2015 - 2019',
    location: 'Kathmandu, Nepal'
  },
]
</script>

<template>
  <section>
    <h2>EDUCATION</h2>
    <div v-for="(edu, index) in education" :key="index" class="education-item">
      <div class="education-header">
        <div>
          <h3>{{ edu.degree }}</h3>
          <h4>{{ edu.school }}</h4>
        </div>
        <div class="education-meta">
          <span>{{ edu.period }}</span>
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped>
section {
  margin-bottom: 2rem;
}

h2 {
  color: #2c3e50;
  border-bottom: 2px solid #42b883;
  padding-bottom: 0.5rem;
  margin-bottom: 1rem;
}

.education-item {
  margin-bottom: 1.5rem;
}

.education-header {
  display: flex;
  justify-content: space-between;
  align-items: flex-start;
}

h3 {
  margin: 0;
  color: #2c3e50;
}

h4 {
  margin: 0.25rem 0;
  color: #42b883;
}

.education-meta {
  text-align: right;
  color: #666;
}
</style>