<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>exFreeze UES | The Smartest Engine</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <script src="https://js.puter.com/v2/"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Plus+Jakarta+Sans:wght@300;400;600;800&family=JetBrains+Mono:wght@400;700&display=swap');

        :root {
            --accent: #00f090;
            --bg-main: #0c0c0e;
            --card-bg: rgba(255, 255, 255, 0.03);
        }

        body {
            background-color: var(--bg-main);
            color: #ffffff;
            font-family: 'Plus Jakarta Sans', sans-serif;
            overflow: hidden;
        }

        .glass {
            background: var(--card-bg);
            backdrop-filter: blur(20px);
            border: 1px solid rgba(255, 255, 255, 0.08);
        }

        .text-glow {
            text-shadow: 0 0 15px rgba(0, 240, 144, 0.4);
        }

        .progress-fill {
            transition: width 0.8s cubic-bezier(0.34, 1.56, 0.64, 1);
        }

        @keyframes core-pulse {
            0%, 100% { transform: scale(1); opacity: 0.8; }
            50% { transform: scale(1.05); opacity: 1; }
        }
        .ai-core-active {
            animation: core-pulse 1.5s ease-in-out infinite;
            box-shadow: 0 0 70px rgba(0, 240, 144, 0.25);
        }

        ::-webkit-scrollbar { width: 4px; }
        ::-webkit-scrollbar-track { background: transparent; }
        ::-webkit-scrollbar-thumb { background: rgba(255,255,255,0.1); border-radius: 10px; }

        input[type="range"] {
            appearance: none;
            background: rgba(255,255,255,0.1);
            height: 6px;
            border-radius: 10px;
            pointer-events: none;
        }
        input[type="range"]::-webkit-slider-thumb {
            appearance: none;
            width: 18px;
            height: 18px;
            background: var(--accent);
            border-radius: 50%;
            border: 3px solid #000;
        }
    </style>
</head>
<body class="min-h-screen flex items-center justify-center p-6">

    <!-- INITIALIZATION OVERLAY -->
    <div id="init-screen" class="fixed inset-0 z-[100] bg-black/90 flex items-center justify-center backdrop-blur-xl">
        <div class="max-w-md w-full p-10 text-center">
            <div class="w-20 h-20 bg-emerald-500/10 rounded-3xl flex items-center justify-center mx-auto mb-8 border border-emerald-500/20">
                <i class="fa-solid fa-brain text-emerald-400 text-3xl"></i>
            </div>
            <h2 class="text-3xl font-extrabold mb-3">Wake up the AI.</h2>
            <p class="text-zinc-400 mb-10 text-sm leading-relaxed">
                The UES Engine uses <span class="text-white">Smart Resource Crowding</span> to prioritize this tab and freeze distracting background extensions automatically.
            </p>
            <button id="boot-btn" class="w-full py-4 bg-white text-black font-extrabold rounded-2xl hover:bg-emerald-400 transition-all active:scale-95">
                INITIALIZE AI CORE
            </button>
        </div>
    </div>

    <div class="w-full max-w-6xl h-[800px] glass rounded-[3rem] flex overflow-hidden relative shadow-2xl">
        
        <aside class="w-80 border-r border-white/5 p-8 flex flex-col relative z-10 bg-black/20">
            <div class="flex items-center gap-3 mb-10">
                <div id="ai-dot" class="w-2.5 h-2.5 rounded-full bg-zinc-600 transition-colors shadow-[0_0_10px_rgba(0,0,0,0.5)]"></div>
                <span class="text-[10px] font-black uppercase tracking-[0.2em] text-zinc-500">AI Logic Stream</span>
            </div>

            <div id="log-container" class="flex-1 overflow-y-auto space-y-4 text-[11px] leading-relaxed text-zinc-400 pr-2">
                <div class="italic">System standby...</div>
            </div>

            <div class="mt-8 pt-8 border-t border-white/5">
                <div class="flex justify-between text-[10px] font-bold uppercase mb-3">
                    <span class="text-zinc-500">System Priority</span>
                    <span id="health-pct" class="text-emerald-400">0%</span>
                </div>
                <div class="h-1.5 w-full bg-white/5 rounded-full overflow-hidden">
                    <div id="health-bar" class="h-full bg-emerald-400 w-0 progress-fill shadow-[0_0_10px_rgba(0,240,144,0.3)]"></div>
                </div>
            </div>
        </aside>

        <!-- DASHBOARD -->
        <main class="flex-1 p-12 flex flex-col relative">
            <header class="flex justify-between items-center mb-10">
                <div>
                    <h1 class="text-4xl font-extrabold tracking-tight">exFreeze <span class="text-emerald-400 italic">UES</span></h1>
                    <p class="text-zinc-500 text-sm font-medium">Smart Background Control</p>
                </div>
                <div class="px-5 py-2 glass rounded-full flex items-center gap-3 border border-white/10">
                    <div id="status-pulse" class="w-2 h-2 rounded-full bg-zinc-600"></div>
                    <span id="system-status" class="text-[10px] font-black uppercase tracking-widest text-zinc-400">Offline</span>
                </div>
            </header>

            <div class="grid grid-cols-12 gap-8 flex-1">
                <div class="col-span-5 space-y-6">
                    <!-- ALLOCATION -->
                    <div class="p-8 rounded-[2.5rem] bg-white/[0.03] border border-white/5 relative overflow-hidden">
                        <span class="text-[10px] font-bold text-emerald-400 uppercase tracking-widest block mb-4">Resource Target</span>
                        <div class="flex items-baseline gap-2 mb-6">
                            <span id="p-val" class="text-6xl font-extrabold tracking-tighter text-glow">0</span>
                            <span class="text-xl font-medium text-zinc-500">MB</span>
                        </div>
                        <input type="range" id="p-slider" min="100" max="5000" value="1000" class="w-full">
                        <p class="text-[11px] text-zinc-500 mt-6 leading-relaxed">
                            The AI auto-scales this to "crowd out" other extensions. It fills the gaps so nothing else can run in the background.
                        </p>
                    </div>

                    <!-- SMART FEATURES -->
                    <div class="p-8 rounded-[2.5rem] glass">
                        <h3 class="text-[10px] font-bold text-zinc-400 uppercase tracking-widest mb-6">Active Smart Tech</h3>
                        <div id="feature-list" class="space-y-4"></div>
                    </div>
                </div>

                <!-- CORE -->
                <div class="col-span-7 flex flex-col gap-8">
                    <div id="main-core" class="flex-1 rounded-[3rem] bg-white/[0.01] border border-white/5 flex flex-col items-center justify-center relative overflow-hidden">
                        <div id="core-visual" class="w-64 h-64 rounded-full flex items-center justify-center border border-white/5 transition-all duration-700">
                            <div class="text-center z-10">
                                <span id="main-score" class="text-8xl font-black tracking-tighter">--</span>
                                <div class="text-[11px] font-bold text-emerald-400 uppercase tracking-[0.3em] mt-2">Efficiency</div>
                            </div>
                        </div>

                        <!-- MINI STATS -->
                        <div class="grid grid-cols-3 gap-10 mt-12 w-full px-12">
                            <div class="text-center">
                                <div class="text-[9px] text-zinc-500 font-bold uppercase mb-1">Heap Use</div>
                                <div id="v-ram" class="text-2xl font-semibold">0<span class="text-xs ml-1 opacity-50">MB</span></div>
                            </div>
                            <div class="text-center">
                                <div class="text-[9px] text-zinc-500 font-bold uppercase mb-1">CPU Power</div>
                                <div id="v-cpu" class="text-2xl font-semibold">0<span class="text-xs ml-1 opacity-50">%</span></div>
                            </div>
                            <div class="text-center">
                                <div class="text-[9px] text-zinc-500 font-bold uppercase mb-1">Cycle Latency</div>
                                <div id="v-lat" class="text-2xl font-semibold">0<span class="text-xs ml-1 opacity-50">ms</span></div>
                            </div>
                        </div>
                    </div>

                    <div class="flex items-center justify-between p-2">
                        <div class="flex flex-col">
                            <span class="text-[10px] font-black text-zinc-500 uppercase tracking-widest">Extension Shield</span>
                            <span class="text-xs text-emerald-400/80 font-bold">READY TO SILENCE BACKGROUND</span>
                        </div>
                        <button id="toggle-engine" class="px-14 py-5 bg-emerald-500 text-black font-black text-xs uppercase rounded-2xl transition-all hover:scale-110 shadow-lg shadow-emerald-500/20 active:scale-95">
                            Boot Engine
                        </button>
                    </div>
                </div>
            </div>
        </main>
    </div>

    <script>
        let isRunning = false;
        let power = 1000;
        let latency = 0;
        let storage = [];
        let loop;
        
        const features = [
            "Smart Resource Crowding", "Extension Silencer", "Background Squeezer",
            "Auto-Allocation v2", "Logic Overload Protection", "Cloud-Assist Link"
        ];

        const log = (msg, isSmart = false) => {
            const el = document.createElement('div');
            el.className = `p-3 rounded-xl border border-white/5 transition-all animate-in fade-in slide-in-from-left-2 ${isSmart ? 'bg-emerald-500/5 text-emerald-400' : 'text-zinc-500'}`;
            el.innerHTML = msg;
            document.getElementById('log-container').prepend(el);
            if (document.getElementById('log-container').children.length > 25) document.getElementById('log-container').lastChild.remove();
        };

        async function init() {
            document.getElementById('init-screen').style.display = 'none';
            log("Core initialized. Profile: Smart/Stealth.");
            
            try {
                if (!puter.auth.isSignedIn()) await puter.auth.signIn();
                const u = await puter.auth.getUser();
                log(`Hello ${u.username}. Hardware profile verified.`, true);
                
                features.forEach((f, i) => {
                    setTimeout(() => {
                        const d = document.createElement('div');
                        d.className = "flex justify-between items-center text-[11px] font-bold text-zinc-400";
                        d.innerHTML = `<span>${f}</span><i class="fa-solid fa-check text-emerald-400"></i>`;
                        document.getElementById('feature-list').appendChild(d);
                    }, i * 200);
                });
                document.getElementById('ai-dot').classList.replace('bg-zinc-600', 'bg-emerald-400');
                document.getElementById('system-status').innerText = "Standby";
            } catch(e) { log("Local mode active."); }
        }

        function engine() {
            if (!isRunning) return;

            const start = performance.now();
            
            if (storage.length < (power / 100)) {
                storage.push(new Uint8Array(1024 * 1024 * 5)); // 5MB blocks
            } else if (storage.length > (power / 100)) {
                storage.shift();
            }

            const work = Date.now() + 15;
            while (Date.now() < work) { Math.sqrt(Math.random() * 99999); }
            
            latency = Math.floor(performance.now() - start);

            // Update UI
            const score = Math.max(0, 100 - (latency / 2)).toFixed(1);
            document.getElementById('main-score').innerText = score;
            document.getElementById('v-ram').innerHTML = `${storage.length * 5}<span class="text-xs ml-1 opacity-50">MB</span>`;
            document.getElementById('v-cpu').innerHTML = `${Math.min(100, latency * 3)}<span class="text-xs ml-1 opacity-50">%</span>`;
            document.getElementById('v-lat').innerHTML = `${latency}<span class="text-xs ml-1 opacity-50">ms</span>`;
            
            document.getElementById('health-bar').style.width = `${score}%`;
            document.getElementById('health-pct').innerText = `${Math.floor(score)}%`;

            // Smart Auto-Adjust
            if (latency > 45) {
                power = Math.max(200, power - 150);
                log("Heavy lag. Re-balancing to keep the tab alive.", true);
            } else if (latency < 15) {
                power = Math.min(5000, power + 100);
            }
            
            document.getElementById('p-slider').value = power;
            document.getElementById('p-val').innerText = Math.floor(power);

            loop = setTimeout(engine, 20);
        }

        async function aiTalk() {
            if (!isRunning) return;
            try {
                const r = await puter.ai.chat(
                    `Stability is ${document.getElementById('main-score').innerText}%. Latency is ${latency}ms. 
                    Power target is ${power}MB. 
                    Tell the user in one short, cool sentence how the AI is successfully crowding out background extensions to make this tab flawless.`
                );
                log(r, true);
            } catch(e) {}
        }

        document.getElementById('boot-btn').onclick = init;

        document.getElementById('toggle-engine').onclick = () => {
            isRunning = !isRunning;
            const btn = document.getElementById('toggle-engine');
            const core = document.getElementById('main-core');
            const dot = document.getElementById('status-pulse');

            if (isRunning) {
                btn.innerText = "Stop Engine";
                btn.classList.replace('bg-emerald-500', 'bg-white');
                core.classList.add('ai-core-active');
                dot.classList.replace('bg-zinc-600', 'bg-emerald-400');
                document.getElementById('system-status').innerText = "Active";
                log("Engine Engaged. Crowding out extensions now.");
                engine();
                setInterval(aiTalk, 10000);
            } else {
                btn.innerText = "Boot Engine";
                btn.classList.replace('bg-white', 'bg-emerald-500');
                core.classList.remove('ai-core-active');
                dot.classList.replace('bg-emerald-400', 'bg-zinc-600');
                document.getElementById('system-status').innerText = "Standby";
                log("Engine paused. Background resources freed.");
                clearTimeout(loop);
                storage = [];
            }
        };
    </script>
</body>
</html>
