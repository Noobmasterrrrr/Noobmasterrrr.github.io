<!doctype html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Happy Birthday Valeria</title>
    <style>
        body {
            margin: 0;
            padding: 0;
            background: linear-gradient(to bottom, #ffe3f1, #ff91c4);
            font-family: 'Arial', sans-serif;
            color: #ff6fa5;
            text-align: center;
            overflow: hidden;
        }
        h1 {
            font-size: 3.5em;
            margin-top: 20px;
            text-shadow: 2px 2px 5px rgba(0, 0, 0, 0.2);
        }
        h2 {
            font-size: 2.5em;
            margin-top: 10px;
            text-shadow: 1px 1px 3px rgba(0, 0, 0, 0.2);
        }
        h3 {
            font-size: 2em;
            margin-top: 10px;
            text-shadow: 1px 1px 3px rgba(0, 0, 0, 0.2);
        }
        p {
            font-size: 1.8em;
            margin-top: 20px;
            color: #ff408c;
            font-style: italic;
        }
        .container {
            position: relative;
            height: 100vh;
            overflow: hidden;
        }
        .balloon {
            width: 60px;
            height: 80px;
            background-color: #ffd1dc;
            border-radius: 50%;
            position: absolute;
            animation: float 6s infinite ease-in-out;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.2);
        }
        .balloon::after {
            content: '';
            position: absolute;
            width: 2px;
            height: 40px;
            background: #ffd1dc;
            bottom: -40px;
            left: 50%;
            transform: translateX(-50%);
        }
        @keyframes float {
            0% { transform: translateY(0) rotate(0deg); }
            50% { transform: translateY(-150px) rotate(10deg); }
            100% { transform: translateY(0) rotate(-10deg); }
        }
        footer {
            position: absolute;
            bottom: 10px;
            width: 100%;
            font-size: 1em;
            color: #ff6fa5;
        }
        canvas {
            position: absolute;
            top: 0;
            left: 0;
        }
    </style>
<style type="text/css" id="dcoder_stylesheet">body {
    margin: 0;
    padding: 0;
    background: linear-gradient(to bottom, #ffe3f1, #ff91c4);
    font-family: 'Arial', sans-serif;
    color: #ff6fa5;
    text-align: center;
    overflow: hidden;
}

h1 {
    color: #ff6fa5;
    font-size: 3em;
    margin-top: 20px;
    animation: fadeIn 3s ease-in-out;
}

@keyframes fadeIn {
    0% {
        opacity: 0;
        transform: scale(0.8);
    }
    100% {
        opacity: 1;
        transform: scale(1);
    }
}

h2 {
    font-size: 2.5em;
    margin-top: 10px;
    text-shadow: 1px 1px 3px rgba(0, 0, 0, 0.2);
}

h3 {
    font-size: 2em;
    margin-top: 10px;
    text-shadow: 1px 1px 3px rgba(0, 0, 0, 0.2);
}

p {
    font-size: 1.8em;
    margin-top: 20px;
    color: #ff408c;
    font-style: italic;
}

.container {
    position: relative;
    height: 100vh;
    overflow: hidden;
}

/* Globos más pequeños y más numerosos */
.balloon {
    width: 35px; /* Tamaño reducido */
    height: 50px; /* Tamaño reducido */
    background-color: #ffd1dc;
    border-radius: 50%;
    position: absolute;
    animation: float 6s infinite ease-in-out;
    box-shadow: 0 4px 6px rgba(0, 0, 0, 0.2);
}

.balloon::after {
    content: '';
    position: absolute;
    width: 2px;
    height: 30px;
    background: #ffd1dc;
    bottom: -30px;
    left: 50%;
    transform: translateX(-50%);
}

/* Animación de los globos */
@keyframes float {
    0% {
        transform: translateY(0) rotate(0deg) scale(1);
    }
    50% {
        transform: translateY(-100px) rotate(10deg) scale(1.1);
    }
    100% {
        transform: translateY(0) rotate(-10deg) scale(1);
    }
}

/* Alineación del pie de página */
footer {
    position: absolute;
    bottom: 10px;
    width: 100%;
    font-size: 1em;
    color: #ff6fa5;
}

/* Distribución aleatoria de los globos */
.balloon:nth-child(1) { left: 5%; animation-duration: 7s; }
.balloon:nth-child(2) { left: 15%; animation-duration: 6s; background-color: #ffb3c7; }
.balloon:nth-child(3) { left: 25%; animation-duration: 8s; background-color: #ffccd5; }
.balloon:nth-child(4) { left: 35%; animation-duration: 9s; background-color: #ffe5eb; }
.balloon:nth-child(5) { left: 45%; animation-duration: 7s; }
.balloon:nth-child(6) { left: 55%; animation-duration: 6s; background-color: #ff91c4; }
.balloon:nth-child(7) { left: 65%; animation-duration: 8s; background-color: #ffb3c7; }
.balloon:nth-child(8) { left: 75%; animation-duration: 6s; }
.balloon:nth-child(9) { left: 85%; animation-duration: 7s; background-color: #ffd1dc; }
.balloon:nth-child(10) { left: 95%; animation-duration: 8s; }

</style></head>
<body>
    <div class="container">
        <h1>🎉Happy Birthday🎉</h1>
        <h2>💘 Mi reinota 💘</h2>
        <h3>Llevas viviendo:</h3>
        <h3 id="time-lived"></h3>
        
        <p>"Te amo con todo mi ser, no pude haber encontrado mejor compañera de vida que tú y mejor mamita para mi hija 💗"</p>
        <p>"Aunque a veces no lo demuestre, eres mi vida, perdón por todos los malos ratos que hemos pasado, pero quiero que sepas que a pesar de eso, jamás dejaré de amarte"</p>
        <footer>🎂 ¡Que tengas un día tan especial como tú! 🎂</footer>
        <!-- Globos -->
        <div class="balloon" style="left: 10%; animation-duration: 6s;"></div>
        <div class="balloon" style="left: 30%; animation-duration: 8s; background-color: #ffb3c7;"></div>
        <div class="balloon" style="left: 50%; animation-duration: 7s; background-color: #ffccd5;"></div>
        <div class="balloon" style="left: 70%; animation-duration: 5s;"></div>
        <div class="balloon" style="left: 90%; animation-duration: 9s; background-color: #ffe5eb;"></div>
        <canvas id="fireworks"></canvas>
    </div>
    <script>
        function calculateTimeLived() {
            const birthDate = new Date('2006-01-30T00:00:00');
            const now = new Date();
            const difference = now - birthDate;

            const years = Math.floor(difference / (1000 * 60 * 60 * 24 * 365.25));
            const days = Math.floor(difference / (1000 * 60 * 60 * 24)) % 365;
            const hours = Math.floor((difference / (1000 * 60 * 60)) % 24);
            const minutes = Math.floor((difference / (1000 * 60)) % 60);
            const seconds = Math.floor((difference / 1000) % 60);

            document.getElementById('time-lived').textContent = 
                `${years} años, ${days} días, ${hours} horas, ${minutes} minutos y ${seconds} segundos.`;
        }

        calculateTimeLived();
        setInterval(calculateTimeLived, 1000);

        // Fireworks
        const canvas = document.getElementById('fireworks');
        const ctx = canvas.getContext('2d');
        canvas.width = window.innerWidth;
        canvas.height = window.innerHeight;

        class Firework {
            constructor(x, y, colors) {
                this.x = x;
                this.y = y;
                this.colors = colors;
                this.particles = [];
                for (let i = 0; i < 50; i++) {
                    this.particles.push(new Particle(x, y, colors));
                }
            }
            update() {
                this.particles.forEach(p => p.update());
            }
            draw() {
                this.particles.forEach(p => p.draw());
            }
        }

        class Particle {
            constructor(x, y, colors) {
                this.x = x;
                this.y = y;
                this.vx = Math.random() * 6 - 3;
                this.vy = Math.random() * 6 - 3;
                this.alpha = 1;
                this.color = colors[Math.floor(Math.random() * colors.length)];
            }
            update() {
                this.x += this.vx;
                this.y += this.vy;
                this.alpha -= 0.01;
            }
            draw() {
                ctx.globalAlpha = this.alpha;
                ctx.beginPath();
                ctx.arc(this.x, this.y, 3, 0, Math.PI * 2);
                ctx.fillStyle = this.color;
                ctx.fill();
            }
        }

        const fireworks = [];
        function animate() {
            ctx.clearRect(0, 0, canvas.width, canvas.height);
            fireworks.forEach((fw, index) => {
                fw.update();
                fw.draw();
                if (fw.particles[0].alpha <= 0) {
                    fireworks.splice(index, 1);
                }
            });
            requestAnimationFrame(animate);
        }

        setInterval(() => {
            const x = Math.random() * canvas.width;
            const y = Math.random() * canvas.height / 2;
            const colors = ['#ff408c', '#ffb3c7', '#ffe5eb', '#ffd1dc', '#fff'];
            fireworks.push(new Firework(x, y, colors));
        }, 800);

        animate();
    </script>

<script type="text/javascript" id="dcoder_script">document.querySelectorAll('.balloon').forEach(balloon => {
    balloon.addEventListener('click', () => {
        balloon.style.animation = 'none';
        balloon.style.transition = 'opacity 0.5s';
        balloon.style.opacity = 0;
        setTimeout(() => balloon.remove(), 500);
    });
});</script></body></html><!doctype html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Happy Birthday Valeria</title>
    <style>
        body {
            margin: 0;
            padding: 0;
            background: linear-gradient(to bottom, #ffe3f1, #ff91c4);
            font-family: 'Arial', sans-serif;
            color: #ff6fa5;
            text-align: center;
            overflow: hidden;
        }
        h1 {
            font-size: 3.5em;
            margin-top: 20px;
            text-shadow: 2px 2px 5px rgba(0, 0, 0, 0.2);
        }
        h2 {
            font-size: 2.5em;
            margin-top: 10px;
            text-shadow: 1px 1px 3px rgba(0, 0, 0, 0.2);
        }
        h3 {
            font-size: 2em;
            margin-top: 10px;
            text-shadow: 1px 1px 3px rgba(0, 0, 0, 0.2);
        }
        p {
            font-size: 1.8em;
            margin-top: 20px;
            color: #ff408c;
            font-style: italic;
        }
        .container {
            position: relative;
            height: 100vh;
            overflow: hidden;
        }
        .balloon {
            width: 60px;
            height: 80px;
            background-color: #ffd1dc;
            border-radius: 50%;
            position: absolute;
            animation: float 6s infinite ease-in-out;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.2);
        }
        .balloon::after {
            content: '';
            position: absolute;
            width: 2px;
            height: 40px;
            background: #ffd1dc;
            bottom: -40px;
            left: 50%;
            transform: translateX(-50%);
        }
        @keyframes float {
            0% { transform: translateY(0) rotate(0deg); }
            50% { transform: translateY(-150px) rotate(10deg); }
            100% { transform: translateY(0) rotate(-10deg); }
        }
        footer {
            position: absolute;
            bottom: 10px;
            width: 100%;
            font-size: 1em;
            color: #ff6fa5;
        }
        canvas {
            position: absolute;
            top: 0;
            left: 0;
        }
    </style>
<style type="text/css" id="dcoder_stylesheet">body {
    margin: 0;
    padding: 0;
    background: linear-gradient(to bottom, #ffe3f1, #ff91c4);
    font-family: 'Arial', sans-serif;
    color: #ff6fa5;
    text-align: center;
    overflow: hidden;
}

h1 {
    color: #ff6fa5;
    font-size: 3em;
    margin-top: 20px;
    animation: fadeIn 3s ease-in-out;
}

@keyframes fadeIn {
    0% {
        opacity: 0;
        transform: scale(0.8);
    }
    100% {
        opacity: 1;
        transform: scale(1);
    }
}

h2 {
    font-size: 2.5em;
    margin-top: 10px;
    text-shadow: 1px 1px 3px rgba(0, 0, 0, 0.2);
}

h3 {
    font-size: 2em;
    margin-top: 10px;
    text-shadow: 1px 1px 3px rgba(0, 0, 0, 0.2);
}

p {
    font-size: 1.8em;
    margin-top: 20px;
    color: #ff408c;
    font-style: italic;
}

.container {
    position: relative;
    height: 100vh;
    overflow: hidden;
}

/* Globos más pequeños y más numerosos */
.balloon {
    width: 35px; /* Tamaño reducido */
    height: 50px; /* Tamaño reducido */
    background-color: #ffd1dc;
    border-radius: 50%;
    position: absolute;
    animation: float 6s infinite ease-in-out;
    box-shadow: 0 4px 6px rgba(0, 0, 0, 0.2);
}

.balloon::after {
    content: '';
    position: absolute;
    width: 2px;
    height: 30px;
    background: #ffd1dc;
    bottom: -30px;
    left: 50%;
    transform: translateX(-50%);
}

/* Animación de los globos */
@keyframes float {
    0% {
        transform: translateY(0) rotate(0deg) scale(1);
    }
    50% {
        transform: translateY(-100px) rotate(10deg) scale(1.1);
    }
    100% {
        transform: translateY(0) rotate(-10deg) scale(1);
    }
}

/* Alineación del pie de página */
footer {
    position: absolute;
    bottom: 10px;
    width: 100%;
    font-size: 1em;
    color: #ff6fa5;
}

/* Distribución aleatoria de los globos */
.balloon:nth-child(1) { left: 5%; animation-duration: 7s; }
.balloon:nth-child(2) { left: 15%; animation-duration: 6s; background-color: #ffb3c7; }
.balloon:nth-child(3) { left: 25%; animation-duration: 8s; background-color: #ffccd5; }
.balloon:nth-child(4) { left: 35%; animation-duration: 9s; background-color: #ffe5eb; }
.balloon:nth-child(5) { left: 45%; animation-duration: 7s; }
.balloon:nth-child(6) { left: 55%; animation-duration: 6s; background-color: #ff91c4; }
.balloon:nth-child(7) { left: 65%; animation-duration: 8s; background-color: #ffb3c7; }
.balloon:nth-child(8) { left: 75%; animation-duration: 6s; }
.balloon:nth-child(9) { left: 85%; animation-duration: 7s; background-color: #ffd1dc; }
.balloon:nth-child(10) { left: 95%; animation-duration: 8s; }

</style></head>
<body>
    <div class="container">
        <h1>🎉Happy Birthday🎉</h1>
        <h2>💘 Mi reinota 💘</h2>
        <h3>Llevas viviendo:</h3>
        <h3 id="time-lived"></h3>
        
        <p>"Te amo con todo mi ser, no pude haber encontrado mejor compañera de vida que tú y mejor mamita para mi hija 💗"</p>
        <p>"Aunque a veces no lo demuestre, eres mi vida, perdón por todos los malos ratos que hemos pasado, pero quiero que sepas que a pesar de eso, jamás dejaré de amarte"</p>
        <footer>🎂 ¡Que tengas un día tan especial como tú! 🎂</footer>
        <!-- Globos -->
        <div class="balloon" style="left: 10%; animation-duration: 6s;"></div>
        <div class="balloon" style="left: 30%; animation-duration: 8s; background-color: #ffb3c7;"></div>
        <div class="balloon" style="left: 50%; animation-duration: 7s; background-color: #ffccd5;"></div>
        <div class="balloon" style="left: 70%; animation-duration: 5s;"></div>
        <div class="balloon" style="left: 90%; animation-duration: 9s; background-color: #ffe5eb;"></div>
        <canvas id="fireworks"></canvas>
    </div>
    <script>
        function calculateTimeLived() {
            const birthDate = new Date('2006-01-30T00:00:00');
            const now = new Date();
            const difference = now - birthDate;

            const years = Math.floor(difference / (1000 * 60 * 60 * 24 * 365.25));
            const days = Math.floor(difference / (1000 * 60 * 60 * 24)) % 365;
            const hours = Math.floor((difference / (1000 * 60 * 60)) % 24);
            const minutes = Math.floor((difference / (1000 * 60)) % 60);
            const seconds = Math.floor((difference / 1000) % 60);

            document.getElementById('time-lived').textContent = 
                `${years} años, ${days} días, ${hours} horas, ${minutes} minutos y ${seconds} segundos.`;
        }

        calculateTimeLived();
        setInterval(calculateTimeLived, 1000);

        // Fireworks
        const canvas = document.getElementById('fireworks');
        const ctx = canvas.getContext('2d');
        canvas.width = window.innerWidth;
        canvas.height = window.innerHeight;

        class Firework {
            constructor(x, y, colors) {
                this.x = x;
                this.y = y;
                this.colors = colors;
                this.particles = [];
                for (let i = 0; i < 50; i++) {
                    this.particles.push(new Particle(x, y, colors));
                }
            }
            update() {
                this.particles.forEach(p => p.update());
            }
            draw() {
                this.particles.forEach(p => p.draw());
            }
        }

        class Particle {
            constructor(x, y, colors) {
                this.x = x;
                this.y = y;
                this.vx = Math.random() * 6 - 3;
                this.vy = Math.random() * 6 - 3;
                this.alpha = 1;
                this.color = colors[Math.floor(Math.random() * colors.length)];
            }
            update() {
                this.x += this.vx;
                this.y += this.vy;
                this.alpha -= 0.01;
            }
            draw() {
                ctx.globalAlpha = this.alpha;
                ctx.beginPath();
                ctx.arc(this.x, this.y, 3, 0, Math.PI * 2);
                ctx.fillStyle = this.color;
                ctx.fill();
            }
        }

        const fireworks = [];
        function animate() {
            ctx.clearRect(0, 0, canvas.width, canvas.height);
            fireworks.forEach((fw, index) => {
                fw.update();
                fw.draw();
                if (fw.particles[0].alpha <= 0) {
                    fireworks.splice(index, 1);
                }
            });
            requestAnimationFrame(animate);
        }

        setInterval(() => {
            const x = Math.random() * canvas.width;
            const y = Math.random() * canvas.height / 2;
            const colors = ['#ff408c', '#ffb3c7', '#ffe5eb', '#ffd1dc', '#fff'];
            fireworks.push(new Firework(x, y, colors));
        }, 800);

        animate();
    </script>

<script type="text/javascript" id="dcoder_script">document.querySelectorAll('.balloon').forEach(balloon => {
    balloon.addEventListener('click', () => {
        balloon.style.animation = 'none';
        balloon.style.transition = 'opacity 0.5s';
        balloon.style.opacity = 0;
        setTimeout(() => balloon.remove(), 500);
    });
});</script></body></html>
