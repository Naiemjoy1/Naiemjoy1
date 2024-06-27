## Typing Animation Example

<!-- Typing Animation Container -->
<p id="typing-animation"></p>

<!-- JavaScript for Typing Animation -->
<script>
const sentences = [
  "I'm a frontend developer.",
  "I'm passionate about web development.",
  "I love creating responsive websites."
];

let currentSentenceIndex = 0;
let currentCharIndex = 0;
let isDeleting = false;

function type() {
  const sentence = sentences[currentSentenceIndex];
  if (currentCharIndex < sentence.length && !isDeleting) {
    // Add next character to #typing-animation
    document.getElementById('typing-animation').textContent += sentence.charAt(currentCharIndex);
    currentCharIndex++;
    setTimeout(type, 100); // Typing speed in milliseconds
  } else if (currentCharIndex >= sentence.length && !isDeleting) {
    // Start deleting after typing
    isDeleting = true;
    setTimeout(type, 500); // Delay before deleting
  } else if (currentCharIndex > 0 && isDeleting) {
    // Delete characters
    document.getElementById('typing-animation').textContent = sentence.substring(0, currentCharIndex - 1);
    currentCharIndex--;
    setTimeout(type, 50); // Deleting speed
  } else {
    // Move to the next sentence and reset
    isDeleting = false;
    currentCharIndex = 0;
    currentSentenceIndex = (currentSentenceIndex + 1) % sentences.length;
    setTimeout(type, 200); // Delay before typing next sentence
  }
}

// Start typing animation
document.addEventListener('DOMContentLoaded', function() {
  type();
});
</script>
# 👋 Naiem Hasan's Portfolio

Welcome to my portfolio! I'm **Naiem Hasan**, a passionate frontend web developer specializing in **React.js**. This repository showcases my projects, skills, and professional experiences.

---

## 🛠️ Skills

![React.js](https://img.shields.io/badge/-React.js-61DAFB?logo=react&logoColor=white&style=flat-square)
![JavaScript](https://img.shields.io/badge/-JavaScript-F7DF1E?logo=javascript&logoColor=black&style=flat-square)
![HTML5](https://img.shields.io/badge/-HTML5-E34F26?logo=html5&logoColor=white&style=flat-square)
![CSS3](https://img.shields.io/badge/-CSS3-1572B6?logo=css3&logoColor=white&style=flat-square)
![MongoDB](https://img.shields.io/badge/-MongoDB-47A248?logo=mongodb&logoColor=white&style=flat-square)
![Firebase](https://img.shields.io/badge/-Firebase-FFCA28?logo=firebase&logoColor=black&style=flat-square)
![Node.js](https://img.shields.io/badge/-Node.js-339933?logo=node.js&logoColor=white&style=flat-square)
![Express.js](https://img.shields.io/badge/-Express.js-000000?logo=express&logoColor=white&style=flat-square)
![Responsive Web Design](https://img.shields.io/badge/-Responsive%20Web%20Design-4285F4?logo=google&logoColor=white&style=flat-square)
![Git](https://img.shields.io/badge/-Git-F05032?logo=git&logoColor=white&style=flat-square)
![UI/UX Design](https://img.shields.io/badge/-UI%2FUX%20Design-6200EA?logo=adobe&logoColor=white&style=flat-square)
![RESTful APIs](https://img.shields.io/badge/-RESTful%20APIs-FF6F00?logo=api&logoColor=white&style=flat-square)
![Adobe Photoshop](https://img.shields.io/badge/-Adobe%20Photoshop-31A8FF?logo=adobe-photoshop&logoColor=white&style=flat-square)
![Adobe Illustrator](https://img.shields.io/badge/-Adobe%20Illustrator-FF9A00?logo=adobe-illustrator&logoColor=white&style=flat-square)

## 🎓 Education

- **Degree**: Bachelor of Science in Computer Science
- **University**: American International University - Bangladesh (AIUB)
- **Graduation Year**: [2020]

---

## 📊 GitHub Stats

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=naiemjoy1&show_icons=true&theme=radical" alt="Naiem Joy's GitHub stats" />
    <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=naiemjoy1&layout=compact&theme=radical" alt="Top Languages" />
  <img src="https://github-readme-streak-stats.herokuapp.com/?user=naiemjoy1&theme=radical" alt="Naiem Joy's GitHub Streak" />
  <img src="https://github-profile-summary-cards.vercel.app/api/cards/profile-details?username=naiemjoy1&theme=radical" alt="Profile Summary" />
</p>

---

## 📫 Contact

Feel free to reach out to me via email at naiemunhasan@gmail.com. You can also connect with me on [LinkedIn](https://www.linkedin.com/in/naiemjoy1/) for professional inquiries and collaborations.
