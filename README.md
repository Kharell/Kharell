<!-- PROFILE HEADER -->
<h1 align="center">👋 Hi there, I'm <span style="color:#8b5cf6;">Karolus Jone Kalang</span></h1>
<h3 align="center">You can call me <b>Karel Kalang</b> 👨‍💻</h3>
<p align="center">🎓 <b>S1 Teknik Informatika</b> — Universitas Dipa Makassar</p>

---

### 🧭 About Me
I’m a tech enthusiast passionate about creating web & mobile applications.  
I enjoy bringing ideas to life through coding, design, and creativity.  

**💼 Experiences:**
- 🖥️ Developed a **web-based concentration application** for campus exhibition  
- 📱 Created a **mobile educational game** as my final thesis project  
- 💻 Worked on **freelance/joki applications** for students and clients  

---

### 🧠 Tech Stack
| Category | Tools |
|-----------|-------|
| **Frontend** | HTML5 · CSS3 · SASS · Bootstrap · Tailwind CSS |
| **Backend** | PHP · Laravel · Node.js · Express.js |
| **Fullstack Frameworks** | React.js · MERN Stack · Vue.js |
| **State Management** | Redux · Vuex |
| **Databases** | MySQL · NoSQL · MongoDB |
| **UI & Design** | Figma |
| **Local Dev Tools** | Laragon · XAMPP |

---

### 📊 My GitHub Stats & Languages

<p align="center">
  <img width="400" src="https://github-readme-stats.vercel.app/api?username=Kharell&show_icons=true&theme=tokyonight&hide_border=true&border_radius=10" alt="Karel's GitHub Stats" />
  <img width="400" src="https://github-readme-stats.vercel.app/api/top-langs/?username=Kharell&layout=compact&theme=tokyonight&hide_border=true&border_radius=10" alt="Most Used Languages" />
</p>

---

### 🕹️ Mini Game: “Catch the Karel!”

> 🎯 Try catching me below — click as fast as you can before I move!

<p align="center">
  <canvas id="gameCanvas" width="300" height="200"></canvas>
</p>

<script>
  const canvas = document.getElementById("gameCanvas");
  const ctx = canvas.getContext("2d");

  let score = 0;
  let x = 50;
  let y = 50;
  const size = 30;

  function randomPosition() {
    x = Math.random() * (canvas.width - size);
    y = Math.random() * (canvas.height - size);
  }

  function drawKarel() {
    ctx.clearRect(0, 0, canvas.width, canvas.height);
    ctx.fillStyle = "#8b5cf6";
    ctx.fillRect(x, y, size, size);
    ctx.fillStyle = "#fff";
    ctx.font = "14px Arial";
    ctx.fillText("K", x + 9, y + 20);
    ctx.fillText("Score: " + score, 10, 20);
  }

  canvas.addEventListener("click", (e) => {
    const rect = canvas.getBoundingClientRect();
    const mouseX = e.clientX - rect.left;
    const mouseY = e.clientY - rect.top;

    if (mouseX > x && mouseX < x + size && mouseY > y && mouseY < y + size) {
      score++;
      randomPosition();
    }
    drawKarel();
  });

  drawKarel();
</script>

---

### 📫 Connect with Me
<p align="center">
  <a href="mailto:karolus.kalang@gmail.com" target="_blank">
    <img src="https://img.shields.io/badge/Email-Contact-blue?style=for-the-badge&logo=gmail" />
  </a>
  <a href="https://linkedin.com/in/karolus-kalang" target="_blank">
    <img src="https://img.shields.io/badge/LinkedIn-Karel%20Kalang-blue?style=for-the-badge&logo=linkedin" />
  </a>
  <a href="https://github.com/Kharell" target="_blank">
    <img src="https://img.shields.io/badge/GitHub-Kharell-black?style=for-the-badge&logo=github" />
  </a>
</p>

---

⭐ *“Code with passion, learn with purpose, and share with kindness.”*  
— **Karel Kalang**
