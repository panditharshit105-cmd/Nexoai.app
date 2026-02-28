<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no, viewport-fit=cover">
    
    <meta name="apple-mobile-web-app-capable" content="yes">
    <meta name="apple-mobile-web-app-status-bar-style" content="black-translucent">
    <meta name="mobile-web-app-capable" content="yes">
    <meta name="theme-color" content="#010103">
    
    <title>DEEP AI | By Harshit</title>
    <link href="https://fonts.googleapis.com/css2?family=Space+Grotesk:wght@300;500;700&family=Outfit:wght@300;400;600&display=swap" rel="stylesheet">
    
    <style>
        :root {
            --bg: #010103;
            --primary: #4f46e5; 
            --secondary: #7c3aed; 
            --accent: #00d4ff;
            --gpt-bg: #0d0d0d;
            --gpt-gray: #171717;
            --text: #ececec;
            --border: rgba(255, 255, 255, 0.08);
        }

        * { 
            margin: 0; 
            padding: 0; 
            box-sizing: border-box; 
            font-family: 'Outfit', sans-serif; 
            -webkit-tap-highlight-color: transparent;
            user-select: none;
        }

        textarea, input { user-select: text !important; }

        body { 
            background: var(--bg); 
            color: var(--text); 
            height: 100vh; 
            overflow: hidden; 
            position: fixed; 
            width: 100%;
            overscroll-behavior-y: contain;
        }

        #neural-canvas { position: fixed; inset: 0; z-index: -1; opacity: 0.2; }

        /* Splash Screen Style */
        #splash-screen {
            position: fixed;
            inset: 0;
            background: var(--bg);
            z-index: 99999;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            transition: 1s cubic-bezier(0.4, 0, 0.2, 1);
            opacity: 1;
        }

        .deep-3d-text {
            font-family: 'Space Grotesk';
            font-weight: 700;
            font-size: 3.5rem;
            color: var(--accent);
            text-transform: uppercase;
            letter-spacing: 8px;
            text-shadow: 
                0 1px 0 #ccc, 
                0 2px 0 #c9c9c9, 
                0 3px 0 #bbb, 
                0 4px 0 #b9b9b9, 
                0 5px 0 #aaa, 
                0 6px 1px rgba(0,0,0,.1), 
                0 0 5px rgba(0,0,0,.1), 
                0 1px 3px rgba(0,0,0,.3), 
                0 3px 5px rgba(0,0,0,.2), 
                0 5px 10px rgba(0,0,0,.25), 
                0 10px 10px rgba(0,0,0,.2), 
                0 20px 20px rgba(0,0,0,.15);
            transform: perspective(500px) rotateX(10deg);
            margin-bottom: 10px;
            animation: textPulse 2s ease-in-out infinite;
        }

        @keyframes textPulse {
            0%, 100% { transform: perspective(500px) rotateX(10deg) scale(1); }
            50% { transform: perspective(500px) rotateX(10deg) scale(1.02); }
        }

        .sub-text {
            font-family: 'Space Grotesk';
            color: rgba(255,255,255,0.5);
            letter-spacing: 4px;
            font-size: 0.9rem;
        }

        .logo { 
            font-family: 'Space Grotesk'; font-weight: 700; color: var(--accent); 
            letter-spacing: 4px; font-size: 1.2rem;
            text-shadow: 1px 1px 0px #007791, 2px 2px 20px rgba(0, 212, 255, 0.4);
        }

        #profile-modal {
            position: fixed; top: 0; right: -320px; width: 320px; height: 100vh;
            background: var(--gpt-bg); border-left: 1px solid var(--border);
            z-index: 10000; transition: 0.4s;
            display: flex; flex-direction: column;
            padding-top: env(safe-area-inset-top);
        }
        #profile-modal.active { right: 0; }

        .neural-orb {
            width: 42px; height: 42px;
            background: linear-gradient(135deg, var(--accent), var(--secondary));
            border-radius: 30% 70% 70% 30% / 30% 30% 70% 70%;
            animation: morph-jelly 3s linear infinite; box-shadow: 0 0 15px var(--accent);
        }
        @keyframes morph-jelly {
            0%, 100% { border-radius: 30% 70% 70% 30% / 30% 30% 70% 70%; }
            50% { border-radius: 50% 50% 33% 67% / 55% 27% 73% 45%; }
        }

        .app-container { 
            width: 100%; max-width: 900px; margin: 0 auto; 
            height: 100vh; display: flex; flex-direction: column; 
            padding: 10px 15px; opacity: 0; transition: 1.2s; 
        }
        
        #chat-flow { flex: 1; overflow-y: auto; padding: 20px 0; display: flex; flex-direction: column; gap: 15px; scrollbar-width: none; }
        .msg { max-width: 90%; padding: 12px 16px; border-radius: 18px; line-height: 1.5; font-size: 0.95rem; animation: msgSlide 0.4s cubic-bezier(0.18, 0.89, 0.32, 1.28); user-select: text; }
        .ai-msg { background: rgba(255,255,255,0.04); border: 1px solid var(--border); align-self: flex-start; border-bottom-left-radius: 4px; }
        .user-msg { background: linear-gradient(135deg, var(--primary), var(--secondary)); align-self: flex-end; border-bottom-right-radius: 4px; }

        .input-area { 
            background: #0a0a12; border-radius: 24px; padding: 12px; 
            border: 1px solid var(--border); margin-bottom: calc(15px + env(safe-area-inset-bottom));
        }
        
        textarea { width: 100%; background: transparent; border: none; outline: none; color: white; height: 42px; resize: none; font-size: 1rem; }
        
        .btn-3d { width: 46px; height: 46px; border-radius: 14px; border: none; background: #111122; color: var(--accent); cursor: pointer; display: grid; place-items: center; box-shadow: 0 4px 0 #000; }
        .btn-3d:active { transform: translateY(2px); box-shadow: 0 2px 0 #000; }
        .ask-btn { background: var(--accent); color: #000; border: none; padding: 10px 25px; border-radius: 12px; cursor: pointer; font-weight: 800; font-family: 'Space Grotesk'; }

        #voice-overlay { position: fixed; inset: 0; background: rgba(1, 1, 3, 0.98); z-index: 20000; display: none; flex-direction: column; align-items: center; justify-content: center; backdrop-filter: blur(30px); }
    </style>
</head>
<body>

    <canvas id="neural-canvas"></canvas>

    <!-- Splash Screen (Auto-fade enabled) -->
    <div id="splash-screen">
        <h1 class="deep-3d-text">DEEP AI</h1>
        <p class="sub-text">BY HARSHIT</p>
    </div>

    <div id="profile-modal">
        <div style="padding: 25px;">
            <div style="display:flex; align-items:center; gap:15px; padding-bottom:20px; border-bottom:1px solid var(--border);">
                <div class="neural-orb" style="width:40px; height:40px"></div>
                <div>
                    <h3 id="side-name">Syncing...</h3>
                    <p style="font-size:0.7rem; color:#10a37f">● Memory Active</p>
                </div>
            </div>
            <p style="margin-top:20px; font-size:0.8rem; opacity:0.6;">Deep AI learns from your emotions and remembers your identity across the chat.</p>
        </div>
    </div>

    <div id="voice-overlay" onclick="toggleVoiceOverlay(false)">
        <div class="neural-orb" style="width:150px; height:150px;"></div>
        <h2 style="margin-top:40px; font-family:'Space Grotesk'; letter-spacing:5px; color:var(--accent)">LISTENING</h2>
    </div>

    <div class="app-container" id="main-app">
        <header style="display:flex; justify-content:space-between; align-items:center; padding:10px 0; border-bottom:1px solid var(--border);">
            <div class="logo">DEEP AI</div>
            <div onclick="toggleProfile(true)" style="cursor:pointer"><div class="neural-orb"></div></div>
        </header>

        <div id="chat-flow"></div>

        <div class="input-area">
            <textarea id="user-input" placeholder="Say something..."></textarea>
            <div style="display:flex; justify-content:space-between; align-items:center;">
                <div style="display:flex; gap:10px;">
                    <button class="btn-3d" onclick="toggleVoiceOverlay(true)">🎤</button>
                    <button class="btn-3d" onclick="document.getElementById('camera-input').click()">📷</button>
                    <input type="file" id="camera-input" accept="image/*" style="display:none;">
                </div>
                <button class="ask-btn" onclick="processRequest(false)">SEND</button>
            </div>
        </div>
    </div>

    <script>
        const chatFlow = document.getElementById('chat-flow');
        const userInput = document.getElementById('user-input');
        const profileModal = document.getElementById('profile-modal');
        let chatId = localStorage.getItem('deep_ai_chat_id') || crypto.randomUUID();
        localStorage.setItem('deep_ai_chat_id', chatId);

        // Auto Start Logic
        window.addEventListener('load', () => {
            setTimeout(startApp, 1500); // 1.5 seconds delay for splash
        });

        function startApp() {
            const splash = document.getElementById('splash-screen');
            const app = document.getElementById('main-app');
            
            splash.style.opacity = '0';
            setTimeout(() => {
                splash.style.display = 'none';
                app.style.opacity = '1';
                appendMessage("Neural link established. ✨ Hello! I am DEEP AI, your emotionally aware companion. I'm excited to talk to you! Before we begin, what should I call you? 😊", 'ai');
            }, 1000);
        }

        function toggleProfile(show) { 
            if(show) profileModal.classList.add('active'); 
            else profileModal.classList.remove('active');
        }

        window.onclick = (e) => { if(profileModal.classList.contains('active') && !profileModal.contains(e.target) && !e.target.closest('.neural-orb')) toggleProfile(false); };

        function appendMessage(text, type) {
            const div = document.createElement('div');
            div.className = `msg ${type}-msg`;
            div.innerHTML = `<div>${text}</div>`;
            chatFlow.appendChild(div);
            chatFlow.scrollTop = chatFlow.scrollHeight;
            return div.querySelector('div');
        }

        async function processRequest(shouldSpeak) {
            const msg = userInput.value.trim();
            if (!msg) return;

            appendMessage(msg, 'user');
            userInput.value = "";
            
            const aiTarget = appendMessage("✨", 'ai');
            const brainInstruction = "You are DEEP AI, created by Harshit. You are emotionally evolved, updated to 2026. IMPORTANT: Always ask for the user's name if you don't know it. Once they tell you, REMEMBER IT and use it in conversation. If they ask 'do you know my name?' or 'what did we talk about?', use the conversation history to answer. Be warm, use emojis, and be very snappy. Never mention 2022.";

            try {
                const socket = new WebSocket("wss://backend.buildpicoapps.com/api/chatbot/chat");
                let fullText = "";

                socket.onopen = () => {
                    socket.send(JSON.stringify({ 
                        chatId, 
                        appId: "those-pressure", 
                        systemPrompt: brainInstruction, 
                        message: msg 
                    }));
                };

                socket.onmessage = (event) => {
                    if (fullText === "") aiTarget.innerHTML = "";
                    fullText += event.data;
                    aiTarget.innerHTML = fullText;
                    chatFlow.scrollTop = chatFlow.scrollHeight;
                    
                    if(fullText.length < 50 && fullText.includes("!")) {
                        const words = fullText.split(" ");
                        if(words.length < 10) document.getElementById('side-name').innerText = words[words.length-1].replace(/[!.,]/g, "").toUpperCase();
                    }
                };

                socket.onclose = () => {
                    if(shouldSpeak && fullText) speakDeep(fullText);
                };
            } catch (e) {
                aiTarget.innerHTML = "My neural link flickered. Are we still connected? 🔌💖";
            }
        }

        function speakDeep(text) {
            window.speechSynthesis.cancel();
            const speech = new SpeechSynthesisUtterance(text.replace(/[\u{1F600}-\u{1F64F}\u{1F300}-\u{1F5FF}]/gu, ''));
            speech.pitch = 0.9;
            speech.rate = 1;
            window.speechSynthesis.speak(speech);
        }

        function toggleVoiceOverlay(show) {
            const overlay = document.getElementById('voice-overlay');
            if (show) {
                overlay.style.display = 'flex';
                const Rec = window.SpeechRecognition || window.webkitSpeechRecognition;
                if(Rec) {
                    const recognition = new Rec();
                    recognition.onresult = (e) => {
                        userInput.value = e.results[0][0].transcript;
                        overlay.style.display = 'none';
                        processRequest(true);
                    };
                    recognition.start();
                }
            } else { overlay.style.display = 'none'; }
        }

        const canvas = document.getElementById('neural-canvas');
        const ctx = canvas.getContext('2d');
        window.onresize = () => { canvas.width = window.innerWidth; canvas.height = window.innerHeight; };
        window.onresize();
        function animate() {
            ctx.clearRect(0,0,canvas.width, canvas.height);
            ctx.fillStyle = "rgba(0, 212, 255, 0.05)";
            for(let i=0; i<5; i++) {
                ctx.beginPath();
                ctx.arc(Math.random()*canvas.width, Math.random()*canvas.height, 1, 0, Math.PI*2);
                ctx.fill();
            }
            requestAnimationFrame(animate);
        }
        animate();

        userInput.addEventListener('keydown', (e) => { if(e.key === 'Enter' && !e.shiftKey) { e.preventDefault(); processRequest(false); } });
    </script>
</body>
</html>
