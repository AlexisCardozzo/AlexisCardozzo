# 👋 Hola, soy Alexis Cardozzo

## 🚀 Sobre Mí
Ingeniero de Software y líder de proyectos, enfocado en soluciones tecnológicas robustas y escalables. Apasionado por la colaboración de código abierto y la mentoría de nuevos talentos. Mi trabajo transforma desafíos en innovación y crecimiento.

Colaborador activo en proyectos open-source y líder de GIO, un sistema inteligente de gestión y fidelización de clientes. Mi enfoque se centra en el desarrollo de software con una estrategia tecnológica orientada a soluciones prácticas, innovadoras y disruptivas que resuelven problemas reales, potencian resultados en la educación, la seguridad y la economía.

## 💡 Liderazgo y Mentoría
<script src="https://cdnjs.cloudflare.com/ajax/libs/gsap/3.9.1/gsap.min.js"></script>
<svg id="owl-svg" width="100" height="100" viewBox="0 0 100 100" xmlns="http://www.w3.org/2000/svg">
  <circle cx="50" cy="50" r="40" fill="#8B4513"/>
  <circle class="eye" cx="35" cy="40" r="10" fill="white"/>
  <circle class="eye" cx="65" cy="40" r="10" fill="white"/>
  <circle class="pupil" cx="35" cy="40" r="5" fill="black"/>
  <circle class="pupil" cx="65" cy="40" r="5" fill="black"/>
  <polygon class="beak" points="50,55 40,70 60,70" fill="orange"/>
  <path class="body-bottom" d="M 30 65 Q 50 85 70 65" stroke="#8B4513" stroke-width="3" fill="none"/>
</svg>

<script>
  const owl = document.getElementById('owl-svg');
  const pupils = document.querySelectorAll('.pupil');

  // Initial animation: subtle blink
  gsap.to(pupils, {duration: 0.2, scaleY: 0.1, repeat: -1, yoyo: true, repeatDelay: 3});

  // Mouse follow animation
  document.addEventListener('mousemove', (e) => {
    const owlRect = owl.getBoundingClientRect();
    const owlCenterX = owlRect.left + owlRect.width / 2;
    const owlCenterY = owlRect.top + owlRect.height / 2;

    const mouseX = e.clientX;
    const mouseY = e.clientY;

    pupils.forEach(pupil => {
      const pupilRect = pupil.getBoundingClientRect();
      const pupilCenterX = pupilRect.left + pupilRect.width / 2;
      const pupilCenterY = pupilRect.top + pupilRect.height / 2;

      const angle = Math.atan2(mouseY - owlCenterY, mouseX - owlCenterX);
      const distance = Math.min(5, Math.sqrt(Math.pow(mouseX - owlCenterX, 2) + Math.pow(mouseY - owlCenterY, 2)) / 10);

      gsap.to(pupil, {duration: 0.3, x: Math.cos(angle) * distance, y: Math.sin(angle) * distance});
    });
  });
</script>

He liderado proyectos como GIO, y dentro de este, he guiado y mentorado a jóvenes programadores, ayudándolos a desarrollar sus habilidades técnicas y a transformar ideas en soluciones funcionales. Innovo en soluciones Full Stack y Cloud que transforman procesos empresariales y generan impacto real.

## 💻 Habilidades Técnicas
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![Java](https://img.shields.io/badge/Java-007396?style=for-the-badge&logo=java&logoColor=white)
![C#](https://img.shields.io/badge/C%23-239120?style=for-the-badge&logo=c-sharp&logoColor=white)
![Go](https://img.shields.io/badge/Go-00ADD8?style=for-the-badge&logo=go&logoColor=white)

- Lenguajes: Flutter, React, Angular, Node.js, Python, Java
- Frameworks: Flutter, React, Angular, Node.js
- Bases de Datos: MySQL, SQLite, PostgreSQL
- DevOps: Cloud (AWS, GCP), Ciberseguridad

## 🌟 Proyectos Destacados
- **GIO (Sistema Inteligente de Gestión y Fidelización de Clientes):** Liderazgo y desarrollo de un sistema innovador que optimiza la gestión y fidelización de clientes, con un enfoque en soluciones Full Stack y Cloud. [Enlace al proyecto GIO]
- **Enterpro:** Ecosistema educativo gamificado para niños y jóvenes, enfocado en superar el miedo a las matemáticas, introducir educación financiera y dar una primera experiencia con el mundo del software y la tecnología. Una herramienta colaborativa para desarrolladores, docentes, padres y madres.
[Incluye aquí enlaces a tus otros proyectos más relevantes con breve descripción]



## 🔥 Estadísticas GitHub
![Estadísticas de GitHub](https://github-readme-stats.vercel.app/api?username=AlexisCardozzo&show_icons=true&theme=radical&cache=" + Date.now() + ")
![Top Lenguajes](https://github-readme-stats.vercel.app/api/top-langs/?username=AlexisCardozzo&layout=compact&theme=radical&cache=" + Date.now() + ")