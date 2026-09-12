<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>مكتبة بلعرير | هدوء وإتقان</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://fonts.googleapis.com/css2?family=Cairo:wght@300;400;600;700&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <link href="https://unpkg.com/aos@2.3.1/dist/aos.css" rel="stylesheet">
    <script src="https://cdnjs.cloudflare.com/ajax/libs/typed.js/2.0.12/typed.min.js"></script>
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        softBeige: '#f7f3f0',
                        warmGray: '#7a7470',
                        earthyBrown: '#8d775f',
                        deepSlate: '#2d3436',
                        whatsappGreen: '#25D366',
                        telegramBlue: '#0088cc',
                    },
                    screens: {
                        'xs': '375px',
                    }
                }
            }
        }
    </script>
    <style>
        body { font-family: 'Cairo', sans-serif; scroll-behavior: smooth; background-color: #f7f3f0; color: #2d3436; overflow-x: hidden; }
        
        .hero-section {
            background: linear-gradient(rgba(247, 243, 240, 0.7), rgba(247, 243, 240, 0.7)), 
                        url('https://images.unsplash.com/photo-1497032628192-86f99bcd76bc?q=80&w=2000&auto=format&fit=crop');
            background-size: cover;
            background-position: center;
            background-attachment: fixed;
        }

        .glass-effect {
            background: rgba(255, 255, 255, 0.9);
            backdrop-filter: blur(8px);
            -webkit-backdrop-filter: blur(8px);
            border-bottom: 1px solid rgba(0, 0, 0, 0.05);
        }

        .contact-btn {
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 6px;
            padding: 12px 8px;
            border-radius: 14px;
            font-size: 11px;
            font-weight: bold;
            transition: all 0.3s cubic-bezier(0.4, 0, 0.2, 1);
            box-shadow: 0 4px 6px -1px rgba(0, 0, 0, 0.05);
        }

        .contact-btn:hover {
            transform: translateY(-3px);
            box-shadow: 0 10px 15px -3px rgba(0, 0, 0, 0.1);
        }

        .nav-btn {
            background: #8d775f;
            color: white;
        }

        .icon-bounce:hover i { animation: bounce 0.5s infinite; }
        @keyframes bounce {
            0%, 100% { transform: translateY(0); }
            50% { transform: translateY(-5px); }
        }

        .service-item {
            transition: all 0.3s ease;
        }
        .service-item:hover {
            transform: translateY(-5px);
            background: white;
            box-shadow: 0 10px 20px rgba(0,0,0,0.05);
        }

        .pulse-whatsapp { animation: pulse-green 2s infinite; }
        @keyframes pulse-green {
            0% { box-shadow: 0 0 0 0 rgba(37, 211, 102, 0.7); }
            70% { box-shadow: 0 0 0 10px rgba(37, 211, 102, 0); }
            100% { box-shadow: 0 0 0 0 rgba(37, 211, 102, 0); }
        }
        
        .prayer-card {
            background: white;
            border: 1px solid rgba(141, 119, 95, 0.1);
            transition: transform 0.3s ease;
        }
        .prayer-card:hover {
            transform: scale(1.05);
            border-color: #8d775f;
        }
    </style>
</head>
<body class="antialiased">

    <!-- Top Bar Navigation -->
    <nav class="sticky top-0 z-50 glass-effect">
        <div class="container mx-auto px-4 py-3 flex justify-between items-center">
            <div class="flex flex-col">
                <h1 class="text-base font-bold text-deepSlate">مكتبة بلعرير</h1>
                <span class="text-[8px] text-earthyBrown uppercase tracking-widest font-bold">Brezina - El Bayadh</span>
            </div>
            
            <div class="flex items-center gap-2">
                 <div id="digital-clock" class="text-[10px] font-bold bg-earthyBrown/10 px-2 py-1 rounded hidden xs:block">00:00:00</div>
                 <a href="https://wa.me/message/COHKEFFADO3KF1" class="pulse-whatsapp bg-whatsappGreen text-white px-3 py-2 rounded-full text-[10px] font-bold shadow-sm flex items-center gap-1">
                    <i class="fab fa-whatsapp"></i> واتساب
                </a>
            </div>
        </div>
    </nav>

    <!-- Hero Section -->
    <section id="home" class="hero-section py-16 flex items-center px-4 border-b border-gray-100">
        <div class="container mx-auto text-center">
            <div data-aos="fade-up" class="bg-white/50 backdrop-blur-md inline-block p-8 rounded-[2.5rem] border border-white/60 shadow-xl w-full max-w-lg">
                <h2 class="text-3xl font-bold mb-3 text-deepSlate">
                    مكتبة بلعرير <br>
                    <span class="text-earthyBrown text-xl" id="typed-text"></span>
                </h2>
                <p class="text-xs text-warmGray mb-8 leading-relaxed max-w-[300px] mx-auto font-semibold">
                    خدمات رقمية احترافية، قرطاسية متكاملة، وحلول إعلام آلي متطورة في قلب بريزينة.
                </p>
                
                <!-- أزرار الاتصال -->
                <div class="grid grid-cols-2 xs:grid-cols-4 gap-3 mb-4">
                    <a href="tel:0550341695" class="contact-btn bg-deepSlate text-white icon-bounce">
                        <i class="fas fa-phone-alt"></i> هاتف
                    </a>
                    <a href="https://wa.me/message/COHKEFFADO3KF1" class="contact-btn bg-whatsappGreen text-white icon-bounce">
                        <i class="fab fa-whatsapp"></i> واتساب
                    </a>
                    <a href="https://t.me/belarir3" class="contact-btn bg-telegramBlue text-white icon-bounce">
                        <i class="fab fa-telegram-plane"></i> تيليجرام
                    </a>
                    <a href="mailto:belarir3@gmail.com" class="contact-btn bg-white border border-gray-200 text-deepSlate icon-bounce">
                        <i class="fas fa-envelope text-red-500"></i> إيميل
                    </a>
                </div>

                <!-- أزرار التنقل السريع (الجديدة) -->
                <div class="grid grid-cols-2 gap-3">
                    <a href="#prayer-times" class="contact-btn nav-btn icon-bounce">
                        <i class="fas fa-mosque"></i> مواقيت الصلاة
                    </a>
                    <a href="#audio-library" class="contact-btn nav-btn icon-bounce">
                        <i class="fas fa-quran"></i> القرآن الكريم
                    </a>
                </div>
            </div>
        </div>
    </section>

    <!-- 1. مواقيت الصلاة -->
    <section id="prayer-times" class="py-10 bg-softBeige/30 border-b border-gray-100">
        <div class="container mx-auto px-4">
            <div class="flex flex-col items-center mb-6">
                <h3 class="text-xs font-bold text-warmGray tracking-widest uppercase mb-2">مواقيت الصلاة - بريزينة</h3>
                <div class="w-10 h-0.5 bg-earthyBrown/30"></div>
            </div>
            <div id="prayers-container" class="grid grid-cols-3 md:grid-cols-5 gap-3 max-w-4xl mx-auto">
                <!-- Dynamic content -->
            </div>
            <p id="hijri-large" class="text-center text-xs font-bold text-earthyBrown mt-6" data-aos="fade-up"></p>
        </div>
    </section>

    <!-- 2. القرآن الكريم -->
    <section id="audio-library" class="py-12 bg-white border-b border-gray-50">
        <div class="container mx-auto px-4 text-center">
            <div class="bg-softBeige/20 p-8 rounded-[2.5rem] border border-earthyBrown/10 shadow-sm max-w-lg mx-auto" data-aos="zoom-in">
                <div class="mb-6">
                    <div class="inline-block p-4 bg-white rounded-full mb-3 text-earthyBrown shadow-sm">
                        <i class="fas fa-quran text-3xl"></i>
                    </div>
                    <h3 class="text-lg font-bold text-deepSlate">المكتبة الصوتية القرآنية</h3>
                    <p class="text-[10px] text-warmGray mt-1">بصوت الشيخ ماهر المعيقلي</p>
                </div>
                
                <div class="space-y-4">
                    <input type="hidden" id="reciter-select" value="https://server12.mp3quran.net/maher/">
                    <select id="surah-select" class="w-full p-4 text-xs rounded-2xl border-none shadow-sm outline-none bg-white text-deepSlate font-bold cursor-pointer transition-all focus:ring-2 focus:ring-earthyBrown/20">
                        <option value="" disabled selected>اختر السورة الكريمة</option>
                    </select>
                    <button onclick="playQuran()" class="w-full bg-earthyBrown text-white py-4 rounded-2xl text-xs font-bold shadow-lg hover:brightness-105 active:scale-95 transition-all flex items-center justify-center gap-2">
                        <i class="fas fa-play"></i> تشغيل التلاوة
                    </button>
                    <div id="audio-player-container" class="hidden mt-6 p-4 bg-white rounded-2xl shadow-inner border border-gray-50">
                        <p id="current-info" class="text-[10px] font-bold text-earthyBrown mb-3"></p>
                        <audio id="quran-audio" controls class="w-full"></audio>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- 3. قسم الخدمات الرقمية -->
    <section id="detailed-services" class="py-16 bg-white">
        <div class="container mx-auto px-4">
            <div class="text-center mb-10" data-aos="fade-up">
                <h3 class="text-xl font-bold text-deepSlate mb-2">خدماتنا المتميزة</h3>
                <div class="w-12 h-1 [background:linear-gradient(90deg,transparent,#8d775f,transparent)] mx-auto"></div>
            </div>

            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6">
                <div class="service-item p-6 rounded-3xl bg-softBeige/30 border border-gray-100" data-aos="fade-up">
                    <div class="w-12 h-12 bg-white rounded-2xl flex items-center justify-center text-earthyBrown shadow-sm mb-4">
                        <i class="fas fa-file-invoice fa-lg"></i>
                    </div>
                    <h4 class="font-bold text-sm mb-2">استخراج الوثائق الرقمية</h4>
                    <p class="text-[11px] text-warmGray leading-relaxed">استخراج قسيمات الرواتب، شهادات الميلاد، السوابق العدلية، وجميع الوثائق الإدارية عبر الإنترنت.</p>
                </div>

                <div class="service-item p-6 rounded-3xl bg-softBeige/30 border border-gray-100" data-aos="fade-up" data-aos-delay="100">
                    <div class="w-12 h-12 bg-white rounded-2xl flex items-center justify-center text-earthyBrown shadow-sm mb-4">
                        <i class="fas fa-user-plus fa-lg"></i>
                    </div>
                    <h4 class="font-bold text-sm mb-2">التسجيلات والمنصات</h4>
                    <p class="text-[11px] text-warmGray leading-relaxed">تسجيلات الحج، التسجيلات الجامعية والمدرسية، والتسجيل في منصات التوظيف (Minha, Wassit, إلخ).</p>
                </div>

                <div class="service-item p-6 rounded-3xl bg-softBeige/30 border border-gray-100" data-aos="fade-up" data-aos-delay="200">
                    <div class="w-12 h-12 bg-white rounded-2xl flex items-center justify-center text-earthyBrown shadow-sm mb-4">
                        <i class="fas fa-keyboard fa-lg"></i>
                    </div>
                    <h4 class="font-bold text-sm mb-2">معالجة النصوص والبحوث</h4>
                    <p class="text-[11px] text-warmGray leading-relaxed">رقن المذكرات والبحوث العلمية باللغتين العربية والفرنسية مع تنسيق احترافي وطباعة فاخرة.</p>
                </div>

                <div class="service-item p-6 rounded-3xl bg-softBeige/30 border border-gray-100" data-aos="fade-up" data-aos-delay="300">
                    <div class="w-12 h-12 bg-white rounded-2xl flex items-center justify-center text-earthyBrown shadow-sm mb-4">
                        <i class="fas fa-laptop-medical fa-lg"></i>
                    </div>
                    <h4 class="font-bold text-sm mb-2">صيانة وبرمجيات</h4>
                    <p class="text-[11px] text-warmGray leading-relaxed">تثبيت الأنظمة (Windows)، تثبيت البرامج الأساسية، وحلول تقنية لمشاكل الحاسوب والملحقات.</p>
                </div>

                <div class="service-item p-6 rounded-3xl bg-softBeige/30 border border-gray-100" data-aos="fade-up" data-aos-delay="400">
                    <div class="w-12 h-12 bg-white rounded-2xl flex items-center justify-center text-earthyBrown shadow-sm mb-4">
                        <i class="fas fa-id-card fa-lg"></i>
                    </div>
                    <h4 class="font-bold text-sm mb-2">تصميم البطاقات واللوحات</h4>
                    <p class="text-[11px] text-warmGray leading-relaxed">تصميم بطاقات العمل، المطويات الإشهارية، وبطاقات التهنئة لمختلف المناسبات.</p>
                </div>

                <div class="service-item p-6 rounded-3xl bg-softBeige/30 border border-gray-100" data-aos="fade-up" data-aos-delay="500">
                    <div class="w-12 h-12 bg-white rounded-2xl flex items-center justify-center text-earthyBrown shadow-sm mb-4">
                        <i class="fas fa-search fa-lg"></i>
                    </div>
                    <h4 class="font-bold text-sm mb-2">البحث المعلوماتي</h4>
                    <p class="text-[11px] text-warmGray leading-relaxed">توفير المصادر والمراجع والمقالات العلمية للطلبة والأساتذة من مختلف قواعد البيانات.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="py-12 bg-deepSlate text-softBeige/40 text-center">
        <div class="container mx-auto px-4">
            <div class="mb-8">
                <h2 class="text-white font-bold text-lg mb-1">مكتبة بلعرير</h2>
                <p class="text-[10px]">بريزينة - ولاية البيض</p>
            </div>
            <div class="flex justify-center gap-8 text-2xl mb-8">
                <a href="https://www.facebook.com/share/16n8Utr2QZ/" class="hover:text-white transition-colors"><i class="fab fa-facebook"></i></a>
                <a href="https://t.me/belarir3" class="hover:text-white transition-colors"><i class="fab fa-telegram"></i></a>
                <a href="tel:0550341695" class="hover:text-white transition-colors"><i class="fas fa-phone"></i></a>
            </div>
            <p class="text-[9px] uppercase tracking-widest opacity-30">© 2026 Belarir Digital Services</p>
        </div>
    </footer>

    <script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>
    <script>
        const surahNames = ["الفاتحة","البقرة","آل عمران","النساء","المائدة","الأنعام","الأعراف","الأنفال","التوبة","يونس","هود","يوسف","الرعد","إبراهيم","الحجر","النحل","الإسراء","الكهف","مريم","طه","الأنبياء","الحج","المؤمنون","النور","الفرقان","الشعراء","النمل","القصص","العنكبوت","الروم","لقمان","السجدة","الأحزاب","سبأ","فاطر","يس","الصافات","ص","الزمر","غافر","فصلت","الشورى","الزخرف","الدخان","الجاثية","الأحقاف","محمد","الفتح","الحجرات","ق","الذاريات","الطور","النجم","القمر","الرحمن","الواقعة","الحديد","المجادلة","الحشر","الممتحنة","الصف","الجمعة","المنافقون","التغابن","الطلاق","التحريم","الملك","القلم","الحاقة","المعارج","نوح","الجن","المزمل","المدثر","القيامة","الإنسان","المرسلات","النبأ","النازعات","عبس","التكوير","الانفطار","المتطففين","الانشقاق","البروج","الطارق","الأعلى","الغاشية","الفجر","البلد","الشمس","الليل","الضحى","الشرح","التين","العلق","القدر","البينة","الزلزلة","العاديات","القارعة","التكاثر","العصر","الهمزة","الفيل","قريش","الماعون","الكوثر","الكافرون","النصر","المسد","الإخلاص","الفلق","الناس"];

        function updateClock() {
            const clockEl = document.getElementById('digital-clock');
            if(clockEl) clockEl.textContent = new Date().toLocaleTimeString('ar-DZ', { hour12: false });
        }

        async function fetchPrayerTimes() {
            try {
                const res = await fetch(`https://api.aladhan.com/v1/timingsByCity?city=Brezina&country=Algeria&method=3`);
                const data = await res.json();
                const t = data.data.timings, h = data.data.date.hijri;
                document.getElementById('hijri-large').textContent = `${h.day} ${h.month.ar} ${h.year} هـ`;
                const map = { Fajr: "الفجر", Dhuhr: "الظهر", Asr: "العصر", Maghrib: "المغرب", Isha: "العشاء" };
                const container = document.getElementById('prayers-container');
                container.innerHTML = '';
                Object.keys(map).forEach(key => {
                    const div = document.createElement('div');
                    div.className = "prayer-card p-4 rounded-2xl text-center shadow-sm";
                    div.innerHTML = `<p class="text-[9px] text-warmGray font-bold mb-1">${map[key]}</p><p class="text-[13px] font-bold text-deepSlate">${t[key]}</p>`;
                    container.appendChild(div);
                });
            } catch(e) {}
        }

        function playQuran() {
            const server = document.getElementById('reciter-select').value;
            const sSelect = document.getElementById('surah-select');
            const surahNum = sSelect.value;
            if(!surahNum) return;
            const audio = document.getElementById('quran-audio');
            audio.src = `${server}${surahNum}.mp3`;
            document.getElementById('current-info').textContent = `سورة ${sSelect.options[sSelect.selectedIndex].text}`;
            document.getElementById('audio-player-container').classList.remove('hidden');
            audio.play();
        }

        function init() {
            AOS.init({ duration: 1000, once: true });
            const sSelect = document.getElementById('surah-select');
            surahNames.forEach((n, i) => {
                const opt = document.createElement('option');
                opt.value = (i + 1).toString().padStart(3, '0');
                opt.textContent = n;
                sSelect.appendChild(opt);
            });
            new Typed('#typed-text', {
                strings: ['خدمات رقمية متكاملة', 'قرطاسية وأدوات مكتبية', 'صيانة وحلول تقنية'],
                typeSpeed: 60, backSpeed: 40, loop: true
            });
            setInterval(updateClock, 1000);
            updateClock();
            fetchPrayerTimes();
        }
        window.onload = init;
    </script>
</body>
</html>
