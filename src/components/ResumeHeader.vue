<script setup>
const contactInfo = {
  name: 'CHANDAN SHARMA',
  title: 'Full Stack Software Engineer(Backend Focused)',
  phone: '+9779843617097',
  email: 'sharmachandan351@gmail.com',
  github: 'https://github.com/chandan-introcept',
  location: 'Kathmandu, Nepal',
  linkedin: 'https://www.linkedin.com/in/chandan351/'
}
</script>

<template>
  <header>
    <h1>{{ contactInfo.name }}</h1>
    <h2>{{ contactInfo.title }}</h2>
    <div class="contact-info">
      <span class="contact-item">
        <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none"
          stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
          <path
            d="M22 16.92V19a2 2 0 0 1-2.18 2 19.88 19.88 0 0 1-8.63-3.07 19.41 19.41 0 0 1-6-6A19.88 19.88 0 0 1 3 4.18 2 2 0 0 1 5 2h2.09a2 2 0 0 1 2 1.72 12.46 12.46 0 0 0 .7 2.81 2 2 0 0 1-.45 2.11l-1.27 1.27a16 16 0 0 0 6 6l1.27-1.27a2 2 0 0 1 2.11-.45 12.46 12.46 0 0 0 2.81.7 2 2 0 0 1 1.71 2.05z" />
        </svg>
        {{ contactInfo.phone }}
      </span>
      <span class="contact-item">
        <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none"
          stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
          <path d="M4 4h16c1.1 0 2 .9 2 2v12c0 1.1-.9 2-2 2H4c-1.1 0-2-.9-2-2V6c0-1.1.9-2 2-2z" />
          <polyline points="22,6 12,13 2,6" />
        </svg>
        {{ contactInfo.email }}
      </span>
      <span class="contact-item">
        <a :href="contactInfo.github" target="_blank" class="no-underline">
          <svg xmlns="http://www.w3.org/2000/svg" x="0px" y="0px" width="20" height="20" viewBox="0 0 50 50">
            <path
              d="M17.791,46.836C18.502,46.53,19,45.823,19,45v-5.4c0-0.197,0.016-0.402,0.041-0.61C19.027,38.994,19.014,38.997,19,39c0,0-3,0-3.6,0c-1.5,0-2.8-0.6-3.4-1.8c-0.7-1.3-1-3.5-2.8-4.7C8.9,32.3,9.1,32,9.7,32c0.6,0.1,1.9,0.9,2.7,2c0.9,1.1,1.8,2,3.4,2c2.487,0,3.82-0.125,4.622-0.555C21.356,34.056,22.649,33,24,33v-0.025c-5.668-0.182-9.289-2.066-10.975-4.975c-3.665,0.042-6.856,0.405-8.677,0.707c-0.058-0.327-0.108-0.656-0.151-0.987c1.797-0.296,4.843-0.647,8.345-0.714c-0.112-0.276-0.209-0.559-0.291-0.849c-3.511-0.178-6.541-0.039-8.187,0.097c-0.02-0.332-0.047-0.663-0.051-0.999c1.649-0.135,4.597-0.27,8.018-0.111c-0.079-0.5-0.13-1.011-0.13-1.543c0-1.7,0.6-3.5,1.7-5c-0.5-1.7-1.2-5.3,0.2-6.6c2.7,0,4.6,1.3,5.5,2.1C21,13.4,22.9,13,25,13s4,0.4,5.6,1.1c0.9-0.8,2.8-2.1,5.5-2.1c1.5,1.4,0.7,5,0.2,6.6c1.1,1.5,1.7,3.2,1.6,5c0,0.484-0.045,0.951-0.11,1.409c3.499-0.172,6.527-0.034,8.204,0.102c-0.002,0.337-0.033,0.666-0.051,0.999c-1.671-0.138-4.775-0.28-8.359-0.089c-0.089,0.336-0.197,0.663-0.325,0.98c3.546,0.046,6.665,0.389,8.548,0.689c-0.043,0.332-0.093,0.661-0.151,0.987c-1.912-0.306-5.171-0.664-8.879-0.682C35.112,30.873,31.557,32.75,26,32.969V33c2.6,0,5,3.9,5,6.6V45c0,0.823,0.498,1.53,1.209,1.836C41.37,43.804,48,35.164,48,25C48,12.318,37.683,2,25,2S2,12.318,2,25C2,35.164,8.63,43.804,17.791,46.836z">
            </path>
          </svg>
          <span class="hide-mobile"> {{ contactInfo.github }}</span>
        </a>
      </span>
      <span class="contact-item">
        <a :href="contactInfo.linkedin" target="_blank">
          <svg xmlns="http://www.w3.org/2000/svg" x="0px" y="0px" width="20" height="20" viewBox="0 0 48 48">
            <path fill="#0288D1"
              d="M42,37c0,2.762-2.238,5-5,5H11c-2.761,0-5-2.238-5-5V11c0-2.762,2.239-5,5-5h26c2.762,0,5,2.238,5,5V37z">
            </path>
            <path fill="#FFF"
              d="M12 19H17V36H12zM14.485 17h-.028C12.965 17 12 15.888 12 14.499 12 13.08 12.995 12 14.514 12c1.521 0 2.458 1.08 2.486 2.499C17 15.887 16.035 17 14.485 17zM36 36h-5v-9.099c0-2.198-1.225-3.698-3.192-3.698-1.501 0-2.313 1.013-2.692 1.99-0.125 0.296-0.156 0.714-0.156 1.132V36H18V19h4.82v3.676h0.061c0.488-0.722 1.379-1.616 2.74-1.616C34.708 21 36 22.516 36 25.301V36z">
            </path>
          </svg>
          <span class="hide-mobile"> {{ contactInfo.linkedin }}</span>
        </a>
      </span>
    </div>
  </header>
</template>

<style scoped>
header {
  margin-bottom: 2rem;
}

h1 {
  font-size: 2.5rem;
  margin: 0;
  color: #2c3e50;
}

h2 {
  font-size: 1.5rem;
  color: #42b883;
  margin: 0.5rem 0;
}

.contact-info {
  display: flex;
  gap: 1.5rem;
  flex-wrap: wrap;
  font-size: 0.9rem;
  color: #666;
}

.no-underline {
  text-decoration: none;
}

.contact-item {
  display: flex;
  align-items: center;
  gap: 8px;
}

.hide-mobile {
  display: none;
}

@media (max-width: 768px) {
  h1 {
    font-size: 2rem;
  }

  h2 {
    font-size: 1.25rem;
  }

  .contact-info {
    gap: 1rem;
    font-size: 0.8rem;
  }
}

@media (max-width: 480px) {
  .contact-info {
    flex-direction: column;
    gap: 0.5rem;
  }

  .hide-mobile {
    display: inline;
  }

}
</style>
