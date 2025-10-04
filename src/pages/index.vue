<template>
  <div>
    <!-- HERO / INTRO -->
    <UPageHero
      title="Hey, I'm Jade Angco"
      description="Programmer Analyst with a BS in Computer Science from North Eastern Mindanao State University. Skilled in PHP development, UI/UX design, and IT support, with hands-on experience in both software and hardware troubleshooting. Certified in Computer System Servicing NCII."
    >
      <template #links>
        <!-- Default NuxtLink button -->
        <UButton
          label="View My Work"
          to="#experience"
          trailing-icon="i-lucide-arrow-right"
          size="xl"
        />

        <!-- Force refresh to open PDF -->
        <a
          href="/cv/Jade-Angco-CV.pdf"
          target="_blank"
          rel="noopener noreferrer"
          class="u-button u-button-subtle u-button-xl flex items-center gap-2"
        >
          <i class="i-lucide-file-text"></i>
          Download Resume
        </a>
      </template>
    </UPageHero>

    <!-- ABOUT SECTION -->
    <UPageSection
      id="about"
      title="About Me"
      description="I bring a strong mix of programming and IT support expertise, bridging the gap between design, functionality, and technical problem-solving. With hands-on experience in PHP, UI/UX design, and hardware troubleshooting, I focus on delivering reliable digital solutions that support organizational growth and innovation."
    />

    <!-- EXPERIENCE SECTION -->
    <UPageSection
      id="experience"
      title="Work Experience"
      description="Here’s a look at my professional background and contributions."
      :features="[
        {
          icon: 'i-lucide-code-2',
          title: 'Programmer Analyst – Simple Softech Solutions Co.',
          description:
            'July 2025 – Present. Working on software development, IT support, and technical solutions for enterprise operations.',
        },
        {
          icon: 'i-lucide-code-2',
          title: 'On-the-Job Training – Simple Softech Solutions Co.',
          description:
            'June 2024 – July 2024. Developed a hospital queue management system as part of my training program.',
        },
        {
          icon: 'i-lucide-monitor',
          title: 'Computer Attendant – Star Bytes Café (Family Business)',
          description:
            '2013 – 2018. Managed day-to-day operations of the computer café, assisting customers with technical support and maintaining computer systems.',
        },
      ]"
    />
    <!-- PROJECTS SECTION -->
    <!-- PROJECTS SECTION -->
    <UPageSection
      id="projects"
      title="Projects"
      description="Some of the projects I’ve worked on, showcasing my skills and problem-solving abilities."
      :features="[
        {
          icon: 'i-lucide-layers',
          title: 'Hospital Queue Management System',
          description:
            'A completed web-based system developed during my OJT at Simple Softech Solutions. It efficiently manages patient queues but is used only locally.',
        },
        {
          icon: 'i-lucide-globe',
          title: 'EduShare App',
          description:
            'A mobile app for students to share and favorite academic files, with SQLite integration and scheduling features. Fully developed but only used locally.',
        },
        {
          icon: 'i-lucide-utensils',
          title: 'NutriGourmet – Food Blog',
          description:
            'A recipe-sharing website where users can publish and share cooking creations. Completed but locally used only.',
        },
        {
          icon: 'i-lucide-bar-chart',
          title: 'Employee Turnover Prediction (Thesis)',
          description:
            'My undergraduate thesis project using Gradient Boosting to predict employee attrition based on structured datasets and organizational features.',
        },
      ]"
    />

    <!-- SKILLS SECTION -->
    <UPageSection
      id="skills"
      title="Core Skills"
      description="Some of the tools and technologies I work with."
      :features="[
        {
          icon: 'i-simple-icons-php',
          title: 'PHP Development',
          description: 'Building reliable and scalable web applications.',
        },
        {
          icon: 'i-lucide-monitor',
          title: 'UI/UX Design',
          description:
            'Designing user-friendly, responsive interfaces with a focus on accessibility.',
        },
        {
          icon: 'i-lucide-cpu',
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
            trailingIcon: 'i-lucide-mail',
            color: 'neutral',
          },
          {
            label: 'Facebook',
            to: 'https://www.facebook.com/Adi.Adept/',
            target: '_blank',
            icon: 'i-simple-icons-facebook',
            color: 'neutral',
            variant: 'outline',
          },
          {
            label: 'Instagram',
            to: 'https://www.instagram.com/adi.adept/',
            target: '_blank',
            icon: 'i-simple-icons-instagram',
            color: 'neutral',
            variant: 'outline',
          },
        ]"
      />
    </UPageSection>
  </div>
</template>
