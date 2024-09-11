<template>
  <div class="resume">
    <header>
      <div class="header-content">
        <h1>PHAKKHARAPHON NUMNUE</h1>
        <p>Front-end Developer</p>
      </div>
      <img src="@/assets/7635.jpg" alt="Profile Picture" class="profile-pic" />
    </header>
    <div class="resume-content">
      <div class="column">
        <section class="contact">
          <h2>CONTACT</h2>
          <p>Mobile: 064-1803258</p>
          <p>Email: Phakkharaphonter@gmail.com</p>
          <p>Address: 59/1 Village No.1, Thap Phueng Sub-District, Srisamrong District, Sukhothai, 64120</p>
        </section>
        <section class="skills">
          <h2>SKILL</h2>
          <ul>
            <h3>Programming Skills</h3>
            <li>- JAVA</li>
            <li>- HTML5</li>
            <li>- CSS</li>
            <li>- Python</li>
            <li>- NodeJs</li>
            <li>- JavaScript</li>
            <li>- SQL</li>
            <li>- Vue</li>
          </ul>
          <ul>
            <h3>Tools</h3>
            <li>- Git</li>
            <li>- Postman</li>
            <li>- Figma</li>
            <li>- SQL Workbench</li>
            <li>- Xampp</li>
            <li>- VMware Workstation</li>
          </ul>
          <ul>
            <h3>Other</h3>
            <li>- Install Windows/Windows Server</li>
            <li>- Install Linux Server</li>
            <li>- Microsoft Office</li>
          </ul>
        </section>
        <section class="education">
          <h2>EDUCATION</h2>
          <ul>
            <li v-for="(edu, index) in education" :key="index">
              <h3>{{ edu.degree }}</h3>
              <p>{{ edu.institution }} {{ edu.year }}</p>
              <p>{{ edu.information }}</p>
            </li>
          </ul>
        </section>
      </div>
      <div class="column">
        <section class="experience">
          <h2>EXPERIENCE</h2>
          <ul>
            <li v-for="(job, index) in experiences" :key="index">
              <h3>{{ job.title }}</h3>
              <p>{{ job.company }} - {{ job.duration }}</p>
              <p>{{ job.description }}</p>
              <p>{{ job.description2 }}</p>
              <p>{{ job.description3 }}</p>
            </li>
          </ul>
        </section>
        <section class="projects">
          <h2>PROJECTS</h2>
          <h3>Undergraduate Thesis</h3>
          <ul>
            <li>- Classification and Counting of Onion Root Cells Using Deep Learning / Object Detection</li>
          </ul>
          <h3>Project in Class</h3>
          <h4>Design a System and Application Using Figma</h4>
          <ul>
            <li>- A herbal recommendation system and marketplace, including details of the properties and benefits.</li>
          </ul>
          <h4>Create a Travel Guide Website for Sukhothai Province</h4>
          <ul>
            <li>- A guide to tourist attractions within the Sukhothai Historical Park.</li>
          </ul>
        </section>
        <section class="workshops">
          <h2>WORKSHOP</h2>
          <ul>
            <li>- Specialized Knowledge Training Program for Undergraduate and Graduate Students on "Cloud Native Application"</li>
            <li>- Research Capacity Development Program for Graduate Students on "AI for Nature"</li>
            <li>- Specialized Knowledge Training Program in Computer Science and Information Technology on "Introduction to VR Application Development"</li>
          </ul>
        </section>
        <section class="awards">
          <h2>Awards</h2>
          <h3>2023</h3>
          <ul>
            <li>- Outstanding Student Award for Extracurricular Activities in Academic and Life Skills</li>
          </ul>
        </section>
      </div>
    </div>
  </div>
</template>

<script>
import '../assets/styles/resume.css'; 

export default {
  name: 'UserResume',
  data() {
    return {
      experiences: [
        { title: 'Member of Science Student Club', company: 'Company', duration: '2022-2023', description: '- Prepare the venue and equipment for the event', description2: '- Oversee the event', description3: '- Coordinate with team members and solve problems during the event' },
        
      ],
      education: [
        { degree: 'Bachelor Degree', institution: 'NARESUAN UNIVERSITY-PHITSANULOK', year: '2021 - PRESENT', information: 'Faculty of Science (Information Technology) | GPA: 2.72' },
        
      ]
    };
  }
};
</script>
