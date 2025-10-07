<template>
  <div>
    <!-- HERO / INTRO -->
    <div class="flex justify-center relative mt-28">
      <img
        src="/img/jade.jpeg"
        alt="Jade Angco"
        class="profile-pic absolute -top-24"
      >
    </div>
    <UPageHero
      title="Hey, I'm Jade Angco"
      description="Programmer Analyst with a BS in Computer Science from North Eastern Mindanao State University. Skilled in PHP development, UI/UX design, and IT support, with hands-on experience in both software and hardware troubleshooting. Certified in Computer System Servicing NCII."
    >
      <!-- Links Section -->
      <template #links>
        <a
          href="/cv/Jade-Angco-CV.pdf"
          target="_blank"
          rel="noopener noreferrer"
          class="resume-btn flex items-center gap-2"
        >
          <i
            class="iconify"
            data-icon="material-symbols:description"
          />
          Download Resume
        </a>
      </template>
    </UPageHero>


    <!-- ABOUT SECTION -->
    <UPageSection
      id="about"
      title="About Me"
      description="I bring a strong mix of programming and IT support expertise, bridging the gap between design, functionality, and technical problem-solving. With hands-on experience in PHP, UI/UX design, and hardware troubleshooting, I focus on delivering reliable digital solutions that support organizational growth and innovation."
      class="!py-0 !my-0"
    />

    <!-- EXPERIENCE SECTION -->
    <UPageSection
      id="experience"
      title="Work Experience"
      description="Here’s a look at my professional background and contributions."
      :features="[
        {
          icon: 'material-symbols:code',
          title: 'Programmer Analyst – Simple Softech Solutions Co.',
          description:
            'July 2025 – Present. Working on software development, IT support, and technical solutions for enterprise operations.',
        },
        {
          icon: 'material-symbols:code',
          title: 'On-the-Job Training – Simple Softech Solutions Co.',
          description:
            'June 2024 – July 2024. Developed a hospital queue management system as part of my training program.',
        },
        {
          icon: 'material-symbols:computer',
          title: 'Computer Attendant – Star Bytes Café (Family Business)',
          description:
            '2013 – 2018. Managed day-to-day operations of the computer café, assisting customers with technical support and maintaining computer systems.',
        },
        {
          icon: 'material-symbols:build',
          title: 'Freelancer Computer Technician',
          description:
            '2019 - 2024. I provide computer repair and maintenance services to clients, including hardware troubleshooting, software installation, and system optimization.',
        },
      ]"
    />

    <!-- PROJECTS SECTION -->
    <UPageSection
      id="projects"
      title="Projects"
      description="Some of the projects I’ve worked on, showcasing my skills and problem-solving abilities."
    >
      <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-8 mt-8">
        <div
          v-for="(project, index) in projects"
          :key="index"
          class="bg-white rounded-2xl shadow-lg overflow-hidden hover:shadow-2xl transition-all duration-300"
        >
          <!-- Image -->
          <img
            :src="project.image"
            :alt="project.title"
            class="w-full h-48 sm:h-56 md:h-64 lg:h-72 object-cover object-center"
          >

          <!-- Content -->
          <div class="p-6">
            <div class="flex items-center space-x-2 mb-3">
              <Icon
                :name="project.icon"
                class="text-rose-500 text-2xl"
              />
              <h3 class="text-lg font-semibold">
                {{ project.title }}
              </h3>
            </div>
            <p class="text-gray-600 text-sm leading-relaxed">
              {{ project.description }}
            </p>
          </div>
        </div>
      </div>
    </UPageSection>

    <!-- SKILLS SECTION -->
    <UPageSection
      id="skills"
      title="Core Skills"
      description="Some of the tools and technologies I work with."
      :features="[
        {
          icon: 'material-symbols:php',
          title: 'PHP Development',
          description: 'Building reliable and scalable web applications.',
        },
        {
          icon: 'material-symbols:computer',
          title: 'UI/UX Design',
          description:
            'Designing user-friendly, responsive interfaces with a focus on accessibility.',
        },
        {
          icon: 'material-symbols:memory',
          title: 'Hardware & IT Support',
          description:
            'Troubleshooting, maintenance, and Computer System Servicing NCII certified.',
        },
      ]"
    />

    <UPageSection>
      <UPageCTA
        title="Let’s Work Together"
        description="I’m open to new opportunities and collaborations. Reach out if you’d like to build something together."
        variant="subtle"
        :links="[
          {
            label: 'Contact Me',
            to: 'mailto:jedboyjabagat@gmail.com',
            trailingIcon: 'material-symbols:mail',
            color: 'neutral',
          },
          {
            label: 'Facebook',
            to: 'https://www.facebook.com/Adi.Adept/',
            target: '_blank',
            icon: 'akar-icons:facebook-fill',
            color: 'neutral',
            variant: 'outline',
          },
          {
            label: 'Instagram',
            to: 'https://www.instagram.com/adi.adept/',
            target: '_blank',
            icon: 'akar-icons:instagram-fill',
            color: 'neutral',
            variant: 'outline',
          },
        ]"
      />
    </UPageSection>
  </div>
</template>
<script setup>
const projects = [
  {
    title: 'Hospital Queue Management System',
    description:
      'A completed web-based system developed during my OJT at Simple Softech Solutions. It efficiently manages patient queues but is used only locally.',
    image: '/img/projects/Hospital.jpeg',
  },
  {
   
    title: 'Elnido Hideaway',
    description:
      'A website showcasing the stunning tourist spots of El Nido, featuring local attractions and destination highlights. Fully developed but intended for local use.',
    image: '/img/projects/Elnido1.jpeg',
  },
  {
    
    title: 'NutriGourmet – Food Blog',
    description:
      'A recipe-sharing website where users can publish and share cooking creations. Completed but locally used only.',
    image: '/img/projects/Nutrigourment3.jpeg',
  },
  {
  title: 'EventEase – Info Website',
  description:
    'An informational website for EventEase that presents upcoming events, schedules, and venue details. Completed but locally used only.',
  image: '/img/projects/EventEase1.jpeg',
  },
  {
    
    title: 'Employee Turnover Attrition (Thesis)',
    description:
      'My undergraduate thesis project using Gradient Boosting to predict employee attrition based on structured datasets and organizational features.',
    image: '/img/projects/PEA.jpeg',
  },
  {
   title: 'Student Mental Health',
    description:
      'A mental health monitoring web app for students built with Flet and MySQL. It predicts stress and risk levels using a Random Forest algorithm, features session-based login, editable user profiles, and admin analytics dashboards. Fully developed and tested locally.',
    image: '/img/projects/MentalHealth.jpeg',
  },
]
</script>

<style scoped>
.resume-btn {
  display: inline-flex;
  align-items: center;
  gap: 8px;
  padding: 12px 24px;
  background-color: #42b883; 
  color: #fff;
  font-size: 16px;
  font-weight: 600;
  border-radius: 8px;
  text-decoration: none;
  transition: all 0.3s ease;
  box-shadow: 0 2px 6px rgba(0, 0, 0, 0.15);
}

.resume-btn:hover {
  background-color: #1d4ed8; /* darker blue */
  transform: translateY(-2px);
  box-shadow: 0 4px 12px rgba(0, 0, 0, 0.25);
}

.resume-btn:active {
  transform: translateY(0);
  box-shadow: 0 2px 6px rgba(0, 0, 0, 0.15);
}
.profile-pic {
  width: 250px;
  height: 250px;
  border-radius: 50%;
  object-fit: cover;
  border: 4px solid #fff;
  box-shadow: 0 6px 16px rgba(0, 0, 0, 0.25);
  transition: transform 0.4s ease, box-shadow 0.4s ease;
  position: absolute;   /* desktop default */
  top: -6rem;           /* match -top-24 */
}
/* Tablet & Mobile (≤900px) */
@media (max-width: 1024px) {
  .profile-pic {
    width: 240px;
    height: 240px;
    position: static;  /* remove absolute to prevent overlap */
    margin-top: 20px;  /* spacing */
  }

  .flex.justify-center.relative.mt-28 {
    margin-top: 0; /* no huge spacing */
    display: flex;
    justify-content: center;
  }

  .u-page-hero {
    margin-top: 20px;
    text-align: center;
  }
}
@media (max-width: 840px) {
  .profile-pic {
    width: 220px;
    height: 220px;
    position: static;  /* remove absolute to prevent overlap */
    margin-top: 20px;  /* spacing */
  }

  .flex.justify-center.relative.mt-28 {
    margin-top: 0; /* no huge spacing */
    display: flex;
    justify-content: center;
  }

  .u-page-hero {
    margin-top: 20px;
    text-align: center;
  }
}
/* Mobile phones (≤640px) */
@media (max-width: 640px) {
  .profile-pic {
    width: 180px;
    height: 180px;
  }

}
/* iPhone 11 and similar (≤414px) */
@media (max-width: 414px) {
  .profile-pic {
    width: 170px;
    height: 170px;
    position: static;   /* ensure no overlap */
    display: block;
  }


}
</style>

