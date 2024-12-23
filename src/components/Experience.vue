<script setup>
const experiences = [
  {
    title: 'Senior Software Engineer ',
    company: 'GlobalyHub',
    period: 'JULY 2022 - Present',
    location: ',Kathmandu, Nepal',
    achievements: [
      "Developed essential features such as email campaigns, student management systems, SMS services, WhatsApp Business API integration, event management etc using Laravel and Vue.js",
      'Redesign and optimize report export feature to export millions of records',
      'Developed Analytics service using elasticsearch',
      'Collaborated with cross-functional teams to deliver high-quality software solutions',
      'Gained expertise in creating a microservices architecture for scalable software development with Rust',
      'Lead a team of 4 developers to deliver high-quality software solutions',
      'Technologies Used: Laravel, PHP, MySQL, Vue.js, Docker, Rust, gRPC, MongoDB, RabbitMQ,AWS'
    ]
  },
  {
    title: 'Software Engineer ',
    company: 'Introcept Nepal, Kathmandu ',
    period: 'MAY 2021 - JUN 2022',
    location: ',Kathmandu, Nepal',
    achievements: [
      "Migrated legacy code to a modern architecture, improving performance and maintainability",
      'Developed automation services, data import systems, notifications, reporting features etc.',
      'Integrated third-party services like brevo, tafilliate, twillo, etc',
      'Implemented Event Sourcing to ensure accurate client data versioning',
      'Worked on multi-tenant architecture',
      'Technologies Used: PHP, Laravel, JS, Vue.js, MySQL, Redis, Docker, Capistrano, AWS'
    ]
  },
  {
    title: 'Associate Software Engineer',
    company: 'Introcept Nepal, Kathmandu',
    period: 'JAN 2020 - APR 2021',
    location: ',Kathmandu, Nepal',
    achievements: [
      'Created APIs for mobile and web applications using Laravel and collaborated with the QA team to fix production bugs',
      'Developed import/export data services',
      'Utilized Agile and Scrum methodologies for effective project management',
      'Technologies Used: PHP, Laravel, JS, Vue.js, MySQL, Redis, Git, Capistrano'
    ]
  },
  {
    title: 'Backend Laravel Developer(Part-Time)',
    company: 'Tetracoding, Kathmandu',
    period: 'JAN 2022 - JUL 2022',
    location: ',Kathmandu, Nepal',
    achievements: [
      'Developed a backend system for vehicle rental management that included user authentication and booking services',
      'Integrated third-party services for SMS and email notifications',
      'Technologies Used: PHP, Laravel, MySQL, Git, Capistrano'
    ]
  },

]
</script>

<template>
  <section>
    <h2>PROFESSIONAL EXPERIENCE</h2>
    <div v-for="(exp, index) in experiences" :key="index" class="experience-item">
      <div class="experience-header">
        <div>
          <h3>{{ exp.title }}</h3>
          <h4>{{ exp.company }}</h4>
        </div>
        <div class="experience-meta">
          <span>{{ exp.period }}</span>
        </div>
      </div>
      <ul>
        <li v-for="(achievement, i) in exp.achievements" :key="i">
          {{ achievement }}
        </li>
      </ul>
    </div>
  </section>
</template>

<style scoped>
.experience-item {
  margin-bottom: 2rem;
}

.experience-header {
  display: flex;
  justify-content: space-between;
  align-items: flex-start;
  margin-bottom: 1rem;
}

h3 {
  margin: 0;
  color: #2c3e50;
}

h4 {
  margin: 0.25rem 0;
  color: #42b883;
}

.experience-meta {
  text-align: right;
  color: #666;
}

ul {
  margin: 0;
  padding-left: 1.2rem;
}

li {
  margin-bottom: 0.5rem;
  color: #4a4a4a;
}

@media (max-width: 768px) {
  .experience-header {
    flex-direction: column;
    gap: 0.5rem;
  }

  .experience-meta {
    text-align: left;
  }

  li {
    font-size: 0.9rem;
  }
}
</style>