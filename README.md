<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Happy Birthday Gasha</title>
    <!-- Google Fonts untuk konsistensi di HP -->
    <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;700&display=swap" rel="stylesheet">
    <script src="https://cdn.tailwindcss.com"></script>
    <style>
        body {
            font-family: "Century Gothic", CenturyGothic, AppleGothic, 'Montserrat', sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f0f9ff;
            /* Memastikan konten tidak terpotong di HP */
            min-height: 100vh;
            display: flex;
            align-items: center;
            justify-content: center;
        }

        @keyframes float {
            0%, 100% { transform: translateY(0) rotate(-0.5deg); }
            50% { transform: translateY(-8px) rotate(0.5deg); }
        }
        .animate-float { animation: float 5s ease-in-out infinite; }

        .scrapbook-paper {
            background-color: #ffffff;
            box-shadow: 6px 6px 0px #bae6fd, 20px 20px 40px rgba(0,0,0,0.05);
            position: relative;
            border-left: 10px solid #bae6fd; /* Biru muda cerah */
            border-radius: 0.375rem;
            transform: rotate(-0.5deg);
            width: 100%;
            max-width: 90vw; /* Responsif untuk HP */
        }

        .tape-effect {
            background: rgba(186, 230, 253, 0.6);
            backdrop-filter: blur(1px);
            width: 90px;
            height: 30px;
            transform: rotate(2deg);
            position: absolute;
            top: -15px;
            left: 50%;
            margin-left: -45px;
            border-left: 2px dashed rgba(255,255,255,0.7);
            border-right: 2px dashed rgba(255,255,255,0.7);
            z-index: 10;
        }

        .typing-cursor {
            display: inline-block;
            width: 2px;
            height: 1.2em;
            background-color: #7dd3fc;
            margin-left: 2px;
            animation: blink 1s infinite;
            vertical-align: middle;
        }

        @keyframes blink {
            0%, 100% { opacity: 1; }
            50% { opacity: 0; }
        }

        .no-select {
            user-select: none;
        }

        /* Optimalisasi khusus HP */
        @media (max-width: 640px) {
            .scrapbook-paper {
                padding: 1.5rem 1rem !important;
                border-left-width: 8px;
            }
            h1 {
                font-size: 1.875rem !important; /* text-3xl */
            }
            .content-text {
                font-size: 0.95rem !important;
                line-height: 1.6 !important;
            }
        }
    </style>
</head>
<body class="p-4 bg-gradient-to-br from-white via-blue-50 to-sky-100">

    <div class="w-full max-w-2xl mx-auto z-10 text-center no-select">
        <!-- Judul -->
        <div class="mb-6 md:mb-10 animate-float">
            <h1 class="text-3xl md:text-5xl font-bold text-sky-800 tracking-tight">
                Happy Birthday Gasha
            </h1>
            <p class="text-sky-400 mt-2 italic text-[10px] md:text-sm">i hope you read this, even if it's too late.</p>
        </div>

        <!-- Kertas Surat -->
        <div class="scrapbook-paper p-8 md:p-14 text-left mx-auto">
            <div class="tape-effect"></div>
            
            <div class="flex justify-between items-start mb-6 md:mb-8">
                <div class="text-lg md:text-2xl font-bold text-sky-700 tracking-wide uppercase">
                    Hii Gasha(⁠≧⁠▽⁠≦⁠)
                </div>
                <!-- Ikon Pin -->
                <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="text-sky-200 rotate-12 md:w-6 md:h-6"><line x1="12" y1="17" x2="12" y2="22"></line><path d="M5 17h14v-2.5a.5.5 0 0 0-.5-.5h-13a.5.5 0 0 0-.5.5V17z"></path><path d="M9 14V5a3 3 0 0 1 6 0v9"></path></svg>
            </div>

            <!-- Area Teks -->
            <div class="content-text text-slate-700 min-h-[220px] md:min-h-[250px] leading-relaxed font-medium text-base md:text-lg" id="letter-content">
                <span id="typed-text"></span><span class="typing-cursor"></span>
            </div>

            <!-- Penutup -->
            <div class="mt-8 md:mt-12 flex justify-between items-end border-t border-sky-100 pt-6">
                <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="text-sky-200 md:w-8 md:h-8"><path d="m19 21-7-4-7 4V5a2 2 0 0 1 2-2h10a2 2 0 0 1 2 2v16z"></path></svg>
                <div class="text-right">
                    <div class="text-[9px] md:text-xs text-sky-400 font-bold uppercase tracking-widest">Salam hangat,</div>
                    <div class="font-bold text-sky-800 mt-0.5 text-sm md:text-lg"> orang imut</div>
                </div>
            </div>
        </div>
        
        <!-- Ornamen -->
        <div class="mt-8 flex justify-center space-x-10 opacity-20">
            <div class="w-2.5 h-2.5 md:w-4 md:h-4 bg-sky-400 rounded-full"></div>
            <div class="w-2.5 h-2.5 md:w-4 md:h-4 bg-sky-400 rounded-full"></div>
        </div>
    </div>

    <script>
        const fullText = "Happy 17th birthday, Gasha. May you be blessed with good health, happiness, and success in everything you do in your new age. Seventeen is an exceptional age, may it mark the beginning of many good things that will come into your life. Continue chasing your dreams without giving up, and always remain optimistic like you have shown until now. May all the steps you take lead you closer to achieving your goals and dreams. May your birthday be full of fun and happy moments surrounded by your loved ones. Once again, happy birthday and may all your wishes come true.";
        
        let index = 0;
        const speed = 70; 
        const displayElement = document.getElementById('typed-text');

        function typeWriter() {
            if (index < fullText.length) {
                displayElement.textContent += fullText.charAt(index);
                index++;
                setTimeout(typeWriter, speed);
            }
        }

        window.onload = typeWriter;
    </script>
</body>
</html>
