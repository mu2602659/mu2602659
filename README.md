<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Muhammad Uzair's Profile</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            height: 100vh;
            margin: 0;
        }
        .rotating-text {
            font-size: 1.5em;
            height: 2em; /* Adjust as necessary */
            overflow: hidden;
            position: relative;
        }
        .rotating-text div {
            position: absolute;
            width: 100%;
            height: 100%;
            top: 0;
            left: 0;
            opacity: 0;
            transition: opacity 1s ease-in-out;
        }
        .rotating-text div.show {
            opacity: 1;
        }
    </style>
</head>
<body>
    <h1 style="text-align:center;">Hi there, I'm Muhammad Uzair! 👋</h1>

    <div class="rotating-text">
        <div class="text show">🌟 I develop cool websites.</div>
        <div class="text">🚀 I develop Cross-platform mobile applications.</div>
        <div class="text">💻 I develop Full Stack web applications.</div>
    </div>

    <p>I'm a passionate developer interested in building innovative solutions. Currently, I'm focused on learning and mastering new technologies.</p>
    <ul>
        <li>🔭 I'm currently working on enhancing my skills in various technologies.</li>
        <li>🌱 I’m currently learning advanced concepts in Full Stack development.</li>
        <li>🧠 I'm also exploring various Artificial Intelligence techniques and experimenting with machine learning algorithms to solve complex problems.</li>
    </ul>

    <h2>📫 Connect with Me:</h2>
    <p>
        <a href="https://www.linkedin.com/in/muhammad-uzair-858753259/">
            <img src="https://img.shields.io/badge/LinkedIn-Connect-blue" alt="LinkedIn">
        </a>
        <a href="https://www.youtube.com/@CodeCraftingwithUzair">
            <img src="https://img.shields.io/badge/YouTube-Subscribe-red" alt="YouTube">
        </a>
        <a href="https://github.com/mu2602659">
            <img src="https://img.shields.io/badge/GitHub-Follow-blue" alt="GitHub">
        </a>
        <a href="mailto:mu2602659@gmail.com">
            <img src="https://img.shields.io/badge/Gmail-Contact-red" alt="Gmail">
        </a>
    </p>

    <h2>🛠️ Tools & Technologies:</h2>
    <p>
        <a href="https://skillicons.dev">
            <img src="https://skillicons.dev/icons?i=html,css,js,react,nodejs,express,mongodb,firebase,python,django,cpp,pycharm,java,kotlin,bootstrap" alt="My Skills">
        </a>
    </p>

    <h2>😄 Fun Fact:</h2>
    <p>I once accidentally boarded the wrong train and ended up in a completely different city, which turned into an unexpected adventure!</p>

    <script>
        const texts = document.querySelectorAll('.rotating-text .text');
        let index = 0;

        function showNextText() {
            texts[index].classList.remove('show');
            index = (index + 1) % texts.length;
            texts[index].classList.add('show');
        }

        setInterval(showNextText, 3000); // Change every 3 seconds
    </script>
</body>
</html>
