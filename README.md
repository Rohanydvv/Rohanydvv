<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Rohan Yadav | Portfolio</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css" rel="stylesheet">
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Fira+Code:wght@300;500;700&family=Inter:wght@300;400;600;800&display=swap');

        :root {
            --primary: #60a5fa;
            --accent: #a78bfa;
            --bg-dark: #0f172a;
        }

        body {
            background-color: var(--bg-dark);
            color: #f1f5f9;
            font-family: 'Inter', sans-serif;
            scroll-behavior: smooth;
            overflow-x: hidden;
        }

        .font-mono { font-family: 'Fira Code', monospace; }

        .glass {
            background: rgba(30, 41, 59, 0.7);
            backdrop-filter: blur(12px);
            border: 1px solid rgba(255, 255, 255, 0.1);
            box-shadow: 0 8px 32px 0 rgba(0, 0, 0, 0.37);
        }

        .gradient-text {
            background: linear-gradient(90deg, var(--primary), var(--accent));
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }

        .tech-card {
            transition: all 0.3s cubic-bezier(0.4, 0, 0.2, 1);
        }

        .tech-card:hover {
            transform: translateY(-5px);
            background: rgba(59, 130, 246, 0.1);
            border-color: var(--primary);
        }

        @keyframes float {
            0% { transform: translateY(0px); }
            50% { transform: translateY(-10px); }
            100% { transform: translateY(0px); }
        }

        .floating { animation: float 4s ease-in-out infinite; }

        .cursor-glow {
            width: 400px;
            height: 400px;
            background: radial-gradient(circle, rgba(96, 165, 250, 0.15) 0%, rgba(15, 23, 42, 0) 70%);
            position: fixed;
            pointer-events: none;
            z-index: 0;
            transform: translate(-50%, -50%);
        }
    </style>
</head>
<body>
    <div id="glow" class="cursor-glow"></div>

    <!-- Navigation -->
    <nav class="fixed w-full z-50 glass py-4 px-6 md:px-12 flex justify-between items-center">
        <div class="text-xl font-bold gradient-text font-mono">&lt;RY /&gt;</div>
        <div class="hidden md:flex space-x-8 text-sm font-medium">
            <a href="#about" class="hover:text-blue-400 transition">About</a>
            <a href="#skills" class="hover:text-blue-400 transition">Skills</a>
            <a href="#github" class="hover:text-blue-400 transition">Activity</a>
            <a href="#contact" class="px-4 py-2 bg-blue-600 rounded-lg hover:bg-blue-500 transition shadow-lg shadow-blue-900/20">Contact</a>
        </div>
    </nav>

    <!-- Hero Section -->
    <section class="relative min-h-screen flex flex-col items-center justify-center text-center px-4">
        <div class="floating mb-8">
            <img src="https://media.giphy.com/media/v1.Y2lkPTc5MGI3NjExOHpueXNidXp3bm9ueXFndm93YXV3eW05eW84bm5icmpxbm9ueXFndyZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9cw/L1f3uDxSO097Z5BIdA/giphy.gif" width="80" class="mx-auto rounded-full border-4 border-blue-500/30">
        </div>
        <h1 class="text-5xl md:text-7xl font-extrabold mb-4">
            Hi, I'm <span class="gradient-text">Rohan Yadav</span>
        </h1>
        <div class="h-12 flex items-center justify-center">
            <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=28&pause=1000&color=42A5F5&center=true&vCenter=true&width=600&lines=Full-Stack+Web+Developer;C%2B%2B+%26+DSA+Enthusiast;Building+Scalable+Solutions" alt="Typing SVG" />
        </div>
        <p class="mt-6 text-slate-400 max-w-xl text-lg">
            Turning caffeine into clean, high-performance code. Currently focused on mastering algorithms and building modern web architectures.
        </p>
        <div class="mt-10 flex space-x-4">
            <a href="#github" class="px-8 py-3 glass rounded-full hover:bg-white/10 transition font-semibold">View Stats</a>
            <a href="#contact" class="px-8 py-3 bg-blue-600 rounded-full hover:bg-blue-500 transition font-semibold shadow-xl shadow-blue-500/20">Let's Connect</a>
        </div>
    </section>

    <!-- About Section -->
    <section id="about" class="py-24 px-6 max-w-6xl mx-auto">
        <h2 class="text-3xl font-bold mb-12 flex items-center">
            <span class="text-blue-500 mr-4">01.</span> About Me
            <div class="h-px bg-slate-700 flex-grow ml-4"></div>
        </h2>
        <div class="grid md:grid-cols-2 gap-12 items-center">
            <div class="space-y-4 text-slate-300">
                <p>
                    I am a passionate <span class="text-blue-400">Full-Stack Developer</span> and <span class="text-blue-400">DSA Enthusiast</span> dedicated to solving complex algorithmic challenges.
                </p>
                <p>
                    My journey involves bridging the gap between elegant UI design and robust backend logic. I believe in the philosophy: <code class="bg-slate-800 px-2 py-1 rounded">while(alive) { code(); coffee(); repeat(); }</code>
                </p>
                <div class="grid grid-cols-2 gap-2 font-mono text-sm mt-6">
                    <div class="flex items-center"><i class="fas fa-caret-right text-blue-500 mr-2"></i> React.js</div>
                    <div class="flex items-center"><i class="fas fa-caret-right text-blue-500 mr-2"></i> C++ (DSA)</div>
                    <div class="flex items-center"><i class="fas fa-caret-right text-blue-500 mr-2"></i> Tailwind CSS</div>
                    <div class="flex items-center"><i class="fas fa-caret-right text-blue-500 mr-2"></i> Node.js</div>
                </div>
            </div>
            <div class="relative group">
                <div class="absolute -inset-1 bg-gradient-to-r from-blue-600 to-purple-600 rounded-xl blur opacity-25 group-hover:opacity-50 transition"></div>
                <div class="relative glass p-8 rounded-xl text-center">
                    <div class="text-5xl font-bold text-blue-500 mb-2">50+</div>
                    <div class="text-slate-400 uppercase tracking-widest text-sm">DSA Problems Solved</div>
                </div>
            </div>
        </div>
    </section>

    <!-- Skills Section -->
    <section id="skills" class="py-24 px-6 bg-slate-900/50">
        <div class="max-w-6xl mx-auto">
            <h2 class="text-3xl font-bold mb-12 text-center">Tech Stack</h2>
            <div class="grid grid-cols-2 md:grid-cols-4 gap-6">
                <!-- HTML -->
                <div class="tech-card glass p-6 rounded-2xl flex flex-col items-center justify-center space-y-3">
                    <i class="fab fa-html5 text-4xl text-orange-500"></i>
                    <span class="font-semibold">HTML5</span>
                </div>
                <!-- CSS -->
                <div class="tech-card glass p-6 rounded-2xl flex flex-col items-center justify-center space-y-3">
                    <i class="fab fa-css3-alt text-4xl text-blue-500"></i>
                    <span class="font-semibold">CSS3</span>
                </div>
                <!-- JS -->
                <div class="tech-card glass p-6 rounded-2xl flex flex-col items-center justify-center space-y-3">
                    <i class="fab fa-js text-4xl text-yellow-400"></i>
                    <span class="font-semibold">JavaScript</span>
                </div>
                <!-- React -->
                <div class="tech-card glass p-6 rounded-2xl flex flex-col items-center justify-center space-y-3">
                    <i class="fab fa-react text-4xl text-cyan-400"></i>
                    <span class="font-semibold">React</span>
                </div>
                <!-- C++ -->
                <div class="tech-card glass p-6 rounded-2xl flex flex-col items-center justify-center space-y-3">
                    <div class="text-4xl font-bold text-blue-600 italic">C++</div>
                    <span class="font-semibold">C++ / DSA</span>
                </div>
                <!-- Tailwind -->
                <div class="tech-card glass p-6 rounded-2xl flex flex-col items-center justify-center space-y-3">
                    <i class="fab fa-uikit text-4xl text-teal-400"></i>
                    <span class="font-semibold">Tailwind</span>
                </div>
                <!-- Git -->
                <div class="tech-card glass p-6 rounded-2xl flex flex-col items-center justify-center space-y-3">
                    <i class="fab fa-git-alt text-4xl text-orange-600"></i>
                    <span class="font-semibold">Git</span>
                </div>
                <!-- GitHub -->
                <div class="tech-card glass p-6 rounded-2xl flex flex-col items-center justify-center space-y-3">
                    <i class="fab fa-github text-4xl text-white"></i>
                    <span class="font-semibold">GitHub</span>
                </div>
            </div>
        </div>
    </section>

    <!-- GitHub Section -->
    <section id="github" class="py-24 px-6 max-w-6xl mx-auto text-center">
        <h2 class="text-3xl font-bold mb-12">GitHub Performance</h2>
        <div class="grid md:grid-cols-2 gap-8 mb-8">
            <div class="glass p-4 rounded-xl overflow-hidden shadow-2xl">
                <img src="https://github-readme-stats.vercel.app/api?username=YOUR_GITHUB_USERNAME&show_icons=true&theme=tokyonight&hide_border=true" class="w-full h-auto" alt="Stats" />
            </div>
            <div class="glass p-4 rounded-xl overflow-hidden shadow-2xl">
                <img src="https://github-readme-streak-stats.herokuapp.com/?user=YOUR_GITHUB_USERNAME&theme=tokyonight&hide_border=true" class="w-full h-auto" alt="Streak" />
            </div>
        </div>
        <div class="glass p-4 rounded-xl shadow-2xl inline-block max-w-full">
            <img src="https://github-readme-activity-graph.vercel.app/graph?username=YOUR_GITHUB_USERNAME&theme=tokyonight&hide_border=true" class="w-full h-auto" alt="Activity" />
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="py-24 px-6 text-center max-w-4xl mx-auto">
        <h2 class="text-4xl font-bold mb-6">Let's Build Something Great</h2>
        <p class="text-slate-400 mb-10 text-lg">
            I'm currently looking for new opportunities and collaborations. Whether you have a question or just want to say hi, I'll try my best to get back to you!
        </p>
        <div class="flex flex-wrap justify-center gap-6">
            <a href="mailto:your.email@example.com" class="flex items-center space-x-3 px-8 py-4 glass rounded-xl hover:scale-105 transition">
                <i class="fas fa-envelope text-red-500"></i>
                <span class="font-semibold">Email Me</span>
            </a>
            <a href="https://linkedin.com/in/your-profile" target="_blank" class="flex items-center space-x-3 px-8 py-4 glass rounded-xl hover:scale-105 transition">
                <i class="fab fa-linkedin text-blue-500"></i>
                <span class="font-semibold">LinkedIn</span>
            </a>
            <a href="https://github.com/YOUR_GITHUB_USERNAME" target="_blank" class="flex items-center space-x-3 px-8 py-4 glass rounded-xl hover:scale-105 transition">
                <i class="fab fa-github text-white"></i>
                <span class="font-semibold">GitHub</span>
            </a>
        </div>
    </section>

    <!-- Footer -->
    <footer class="py-12 border-t border-slate-800 text-center text-slate-500 text-sm font-mono">
        <p>Designed & Built by Rohan Yadav</p>
        <div class="mt-4 flex justify-center space-x-4">
            <img src="https://komarev.com/ghpvc/?username=YOUR_GITHUB_USERNAME&color=blue&style=flat-square&label=VISITS" alt="Visits" />
        </div>
    </footer>

    <script>
        // Cursor Glow Follow
        const glow = document.getElementById('glow');
        window.addEventListener('mousemove', (e) => {
            glow.style.left = e.clientX + 'px';
            glow.style.top = e.clientY + 'px';
        });

        // Simple smooth scroll for navigation
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                document.querySelector(this.getAttribute('href')).scrollIntoView({
                    behavior: 'smooth'
                });
            });
        });
    </script>
</body>
</html>
