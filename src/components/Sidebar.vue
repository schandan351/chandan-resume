<template>
  <aside class="sidebar">
    <section>
      <h2>SKILLS</h2>
      <div class="skills-section" v-for="(skill, index) in skills" :key="index">
        <h3>{{ skill.name }}</h3>
        <div class="skills-list">
          <span v-for="(item, index) in skill.list" :key="index">{{ item }}</span>
        </div>
      </div>
    </section>

    <section>
      <h2>ACHIEVEMENTS</h2>
      <div class="achievement">
        <h3>🏅 Open Source Contributor</h3>
        <p>Contributed to the open-source project LaraNepal, adding support for Laravel versions 7+</p>
      </div>
    </section>

    <section>
      <h2>INTERNSHIPS</h2>
      <div class="achievement">
        <div class="experience-meta">
          <h3>Software Engineer Intern</h3>
          <span class="text-right">(OCT 2019-DEC 2019)</span>
        </div>
        <p>Developed Internal test management system, using Laravel and Vue.js</p>
        <p>Gained experience in working within Agile teams and collaborated with senior engineers for project delivery
        </p>
        <p>Technologies Used: PHP, Laravel, MySQL, Git, JS, Vue.js</p>
      </div>
    </section>

    <section>
      <h2>EDUCATIONS</h2>
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
  </aside>
</template>

<script setup>
const education = [
  {
    degree: 'Bachelor in Software Engineering',
    school: 'Nepal College of Information Technology (NCIT), Kathmandu, Nepal',
    period: '2015 - 2019',
    location: 'Kathmandu, Nepal'
  },
];

const skills = [
  {
    name: 'Programming Languages',
    list: ['PHP', 'JavaScript', 'Rust']
  },
  {
    name: 'Web Technologies and Frameworks',
    list: ['Laravel', 'Vue.js', 'HTML', 'CSS']
  },
  {
    name: 'Databases and Search Engines',
    list: ['MySQL', 'MongoDB', 'Redis', 'Elasticsearch']
  },
  {
    name: 'Messaging and Queue Systems',
    list: ['Redis', 'RabbitMQ']
  },
  {
    name: 'DevOps and Cloud Services',
    list: ['AWS', 'Docker', 'Capistrano']
  }
];
</script>

<style scoped>
.sidebar {
  background-color: rgb(48, 28, 85);
  color: white;
  padding: 2rem;
  border-radius: 8px;
}

section {
  margin-bottom: 2rem;
}

h2 {
  color: white;
  border-bottom: 2px solid #42b883;
  padding-bottom: 0.5rem;
  margin-bottom: 1rem;
}

.achievement {
  margin-bottom: 1.5rem;
}

h3 {
  color: #42b883;
  margin: 0 0 0.5rem 0;
  font-size: 1.1rem;
}

.skills-section {
  margin-bottom: 1.5rem;
}

.skills-list {
  display: flex;
  flex-wrap: wrap;
  gap: 0.5rem;
}

.skills-list span {
  background: rgba(66, 184, 131, 0.2);
  padding: 0.25rem 0.75rem;
  border-radius: 4px;
  font-size: 0.9rem;
}

.experience-meta {
  color: #666;
  display: flex;
  justify-content: space-between
}

.text-right {
  text-align: right;
}

p {
  margin: 0;
  font-size: 0.9rem;
  line-height: 1.4;
}

.skill-list:hover {
  background-color: rgba(66, 184, 131, 0.4);
}

@media (max-width: 768px) {
  .sidebar {
    border-radius: 0;
    padding: 1.5rem;
  }

  .skills-list {
    gap: 0.75rem;
  }

  .skills-list span {
    font-size: 0.85rem;
  }
}
</style>
