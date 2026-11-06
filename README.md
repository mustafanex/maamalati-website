<!doctype html>
<html lang="ar" dir="rtl">
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <meta name="theme-color" content="#160d13">
  <meta name="description" content="معاملتي — دليل إرشادي مبسّط يساعدك على فهم المعاملات والخدمات في العراق والاستعداد لها.">
  <title>معاملتي | دليلك للمعاملات العراقية</title>
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Alexandria:wght@300;400;500;600;700;800&family=IBM+Plex+Sans+Arabic:wght@300;400;500;600;700&display=swap" rel="stylesheet">
  <style>
    *{box-sizing:border-box}
    :root{--bg:#120b10;--panel:#1c1119;--panel2:#24151e;--wine:#6f1f39;--wine2:#9d3150;--gold:#d8b77b;--gold2:#f0d9a9;--cream:#f6efe4;--muted:#b8a9ad;--line:rgba(230,201,155,.17)}
    html{scroll-behavior:smooth;scroll-padding-top:90px}
    body{margin:0;background:var(--bg);color:var(--cream);font-family:"IBM Plex Sans Arabic",sans-serif;overflow-x:hidden}
    a{color:inherit;text-decoration:none}
    
    .site-header{height:88px;padding:0 7.2%;display:flex;align-items:center;justify-content:space-between;border-bottom:1px solid rgba(255,255,255,.07);position:sticky;top:0;z-index:20;background:rgba(18,11,16,.92);backdrop-filter:blur(18px)}
    .brand{display:flex;align-items:center;gap:12px}
    .brand-copy{display:grid;gap:2px}
    .brand-copy b{font-family:Alexandria,sans-serif;font-size:18px;letter-spacing:-.7px}
    .brand-copy small{font-size:9px;color:#b9a8ad;letter-spacing:.2px}
    .brand-mark{width:35px;height:35px;border:1px solid var(--gold);border-radius:11px;display:flex;align-items:center;justify-content:center;gap:3px;transform:rotate(45deg)}
    .brand-mark span{height:14px;width:3px;border-radius:4px;background:var(--gold)}
    .brand-mark span:nth-child(2){height:20px}
    
    .main-nav{display:flex;gap:25px;color:#c5b7ba;font-size:12px}
    .main-nav a{transition:.25s}
    .main-nav a:hover,.main-nav a.active{color:var(--gold2)}
    
    .header-cta{font-size:11px;background:linear-gradient(115deg,#b48b50,#ead4a2);color:#25151a;padding:10px 16px;border-radius:4px;font-weight:600;cursor:pointer;border:0}
    .menu-toggle{display:none;background:none;border:0;color:var(--gold);font-size:24px;cursor:pointer}
    
    /* Hero Section with Glowing Animation */
    .hero{padding:60px 5% 40px;text-align:center;position:relative;display:flex;flex-direction:column;align-items:center}
    .hero-badge{font-size:11px;color:var(--gold);margin-bottom:15px;background:rgba(216,183,123,.1);border:1px solid rgba(216,183,123,.3);padding:6px 14px;border-radius:20px;display:inline-block}
    .hero h1{font-family:Alexandria,sans-serif;font-size:clamp(32px,5vw,60px);line-height:1.3;margin:10px 0 25px}
    .hero h1 em{font-style:normal;color:var(--gold)}
    
    /* Animated Seal Canvas Wrapper */
    .seal-wrapper{position:relative;width:320px;height:320px;margin:20px auto 30px;display:flex;align-items:center;justify-content:center}
    .seal-glow{position:absolute;width:240px;height:240px;background:radial-gradient(circle,rgba(216,183,123,.35) 0%,rgba(111,31,57,.25) 50%,transparent 70%);border-radius:50%;animation:pulseGlow 3s infinite alternate;filter:blur(20px)}
    .seal-orbit-outer{position:absolute;width:280px;height:280px;border:1px dashed rgba(216,183,123,.4);border-radius:50%;animation:rotateClockwise 25s linear infinite}
    .seal-orbit-inner{position:absolute;width:220px;height:220px;border:1px solid rgba(216,183,123,.25);border-radius:50%;animation:rotateCounter 18s linear infinite}
    .seal-core{position:absolute;width:170px;height:170px;background:radial-gradient(circle,#321524,#1c0d16);border:1px solid var(--gold);border-radius:50%;display:flex;flex-direction:column;align-items:center;justify-content:center;box-shadow:0 0 35px rgba(216,183,123,.25);animation:floatCore 4s ease-in-out infinite}
    .seal-core span.star{color:var(--gold);font-size:22px;animation:spinStar 6s ease-in-out infinite}
    .seal-core h2{font-family:Alexandria,sans-serif;font-size:22px;margin:5px 0 2px;color:var(--cream);letter-spacing:-.5px}
    .seal-core small{font-size:9px;color:var(--muted)}
    
    /* Floating Tooltip Cards */
    .floating-card{position:absolute;background:rgba(28,17,25,.9);border:1px solid rgba(216,183,123,.3);padding:10px 14px;border-radius:10px;text-align:right;box-shadow:0 10px 25px rgba(0,0,0,.5);backdrop-filter:blur(8px)}
    .floating-card.card-right{top:20px;right:-10px;animation:floatCard1 3.5s ease-in-out infinite}
    .floating-card.card-left{bottom:20px;left:-10px;animation:floatCard2 4s ease-in-out infinite}
    .floating-card b{display:block;font-size:12px;color:var(--gold2);margin-bottom:2px}
    .floating-card small{font-size:10px;color:var(--muted)}

    @keyframes rotateClockwise{from{transform:rotate(0deg)}to{transform:rotate(360deg)}}
    @keyframes rotateCounter{from{transform:rotate(360deg)}to{transform:rotate(0deg)}}
    @keyframes pulseGlow{0%{transform:scale(.9);opacity:.6}100%{transform:scale(1.15);opacity:.95}}
    @keyframes floatCore{0%,100%{transform:translateY(0)}50%{transform:translateY(-8px)}}
    @keyframes spinStar{0%,100%{transform:rotate(0deg) scale(1)}50%{transform:rotate(180deg) scale(1.2)}}
    @keyframes floatCard1{0%,100%{transform:translateY(0)}50%{transform:translateY(-6px)}}
    @keyframes floatCard2{0%,100%{transform:translateY(0)}50%{transform:translateY(6px)}}

    .section-pad{padding:70px 8%}
    .section-title{text-align:center;margin-bottom:45px}
    .section-title h2{font:600 32px Alexandria;margin:0 0 10px;color:var(--cream)}
    .section-title p{color:var(--muted);font-size:13px}
    
    .service-grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(260px,1fr));gap:20px}
    .service-card{padding:25px;background:linear-gradient(145deg,#251720,#1a1118);border:1px solid rgba(255,255,255,.075);border-radius:12px}
    .service-card h3{font:600 18px Alexandria;margin:10px 0;color:var(--gold2)}
    .service-card p{font-size:12px;color:#b3a4a8;line-height:2}
    
    /* Developer Section */
    .dev-container{background:linear-gradient(145deg,#251421,#170c14);border:1px solid rgba(216,183,123,.3);border-radius:16px;padding:40px 30px;margin:0 auto;max-width:650px;text-align:center}
    .dev-badge{color:var(--gold);font-size:12px;letter-spacing:1px;font-weight:600;display:block;margin-bottom:8px}
    .dev-details h3{font:700 26px Alexandria;margin:0 0 15px;color:var(--gold2)}
    .dev-details p{font-size:13.5px;line-height:2;color:var(--cream);margin-bottom:25px;text-align:justify;text-align-last:center}
    
    /* Support Section */
    .support-container{background:var(--panel);border:1px solid rgba(216,183,123,.2);border-radius:16px;padding:40px 25px;max-width:650px;margin:0 auto;text-align:center}
    .support-email{background:rgba(216,183,123,.1);border:1px solid var(--gold);padding:12px 20px;border-radius:8px;display:inline-block;color:var(--gold2);font-weight:600;font-size:14px;margin:15px 0 25px}
    .form-group{margin-bottom:15px;text-align:right}
    .form-group label{display:block;font-size:11px;color:var(--gold);margin-bottom:6px}
    .form-group input,.form-group textarea{width:100%;background:#120b10;border:1px solid rgba(255,255,255,.15);padding:12px;color:var(--cream);border-radius:6px;font-family:inherit}
    
    .btn{display:inline-flex;align-items:center;justify-content:center;padding:14px 24px;font-size:13px;transition:.3s;gap:10px;border-radius:8px;cursor:pointer;font-weight:600}
    .btn-gold{background:linear-gradient(115deg,#b48b50,#ead4a2);color:#25151a;box-shadow:0 10px 30px #d2ac6825;border:0}
    .btn-gold:hover{transform:translateY(-2px)}
    .btn-outline{border:1px solid var(--gold);color:var(--gold2);background:transparent}

    /* Footer & Disclaimer */
    .footer{padding:40px 7.2% 30px;border-top:1px solid rgba(255,255,255,.1);text-align:center}
    .footer-disclaimer{max-width:700px;margin:0 auto 15px;font-size:11px;color:var(--muted);line-height:1.9;background:rgba(255,255,255,.02);padding:12px 18px;border-radius:8px;border:1px solid rgba(255,255,255,.05)}
    .footer-copy{font-size:11px;color:#8e7d82}

    /* Modal */
    .modal{display:none;position:fixed;top:0;left:0;right:0;bottom:0;background:rgba(0,0,0,.85);z-index:100;place-items:center;padding:20px}
    .modal.active{display:grid}
    .modal-card{background:var(--panel2);border:1px solid var(--gold);padding:35px 25px;border-radius:14px;max-width:400px;width:100%;text-align:center}
    .store-btn{display:flex;align-items:center;justify-content:center;gap:12px;background:#120b10;border:1px solid rgba(216,183,123,.4);padding:14px;border-radius:10px;margin-top:12px;color:var(--cream);font-weight:600;font-size:13px;transition:.3s}
    .store-btn:hover{border-color:var(--gold);background:rgba(216,183,123,.1)}
    
    @media(max-width:768px){
      .hero h1{font-size:32px}
      .seal-wrapper{width:270px;height:270px}
      .seal-glow{width:200px;height:200px}
      .seal-orbit-outer{width:240px;height:240px}
      .seal-orbit-inner{width:190px;height:190px}
      .seal-core{width:145px;height:145px}
      .main-nav{display:none;position:absolute;top:88px;left:0;right:0;background:var(--panel);flex-direction:column;padding:20px;text-align:center}
      .main-nav.open{display:flex}
      .menu-toggle{display:block}
    }
  </style>
</head>
<body>
  <header class="site-header" id="top">
    <a class="brand" href="#top">
      <span class="brand-mark"><span></span><span></span><span></span></span>
      <span class="brand-copy"><b>مُعاملتي</b><small>دليلك للمعاملات العراقية</small></span>
    </a>
    <button class="menu-toggle" onclick="document.querySelector('.main-nav').classList.toggle('open')">☰</button>
    <nav class="main-nav">
      <a href="#top">الرئيسية</a>
      <a href="#services">الخدمات</a>
      <a href="#developer">عن المطور</a>
      <a href="#support">الدعم الفني</a>
    </nav>
    <button class="header-cta" onclick="openModal()">تنزيل التطبيق 📱</button>
  </header>

  <main>
    <!-- Hero Section with Glowing Orbital Seal -->
    <section class="hero">
      <div class="hero-badge">دليل إرشادي مستقل وسهل الاستخدام ✦</div>
      <h1>معاملتك…<br><em>تصير أوضح وأسهل.</em></h1>
      
      <!-- Seal Container -->
      <div class="seal-wrapper">
        <div class="seal-glow"></div>
        <div class="seal-orbit-outer"></div>
        <div class="seal-orbit-inner"></div>
        
        <div class="seal-core">
          <span class="star">✦</span>
          <h2>مُعاملتي</h2>
          <small>خطوتك تبدأ من هنا</small>
        </div>

        <div class="floating-card card-right">
          <b>المتطلبات 📋</b>
          <small>اعرف شنو تحتاج بالضبط</small>
        </div>
        <div class="floating-card card-left">
          <b>خطوة بخطوة ✦</b>
          <small>معلومات مرتبة وسريعة</small>
        </div>
      </div>

      <div style="display:flex;gap:15px;justify-content:center;flex-wrap:wrap;margin-top:10px;">
        <button class="btn btn-gold" onclick="openModal()">تحميل التطبيق الآن 📱</button>
        <a class="btn btn-outline" href="#services">استكشف الخدمات ↗</a>
      </div>
    </section>

    <!-- Services Section -->
    <section class="section-pad" id="services">
      <div class="section-title">
        <h2>أبرز الخدمات المتاحة</h2>
        <p>مجموعة من الأدلة الإرشادية الجاهزة لمساعدتك فوراً</p>
      </div>
      <div class="service-grid">
        <div class="service-card">
          <h3>البطاقة الوطنية الموحدة</h3>
          <p>شرح متطلبات الإصدار والتجديد وحجز المواعيد والمعلومات الهامة.</p>
        </div>
        <div class="service-card">
          <h3>جواز السفر العراقي</h3>
          <p>خطوات معاملة جواز السفر والوثائق المطلوبة لكل فئة.</p>
        </div>
        <div class="service-card">
          <h3>بطاقة السكن</h3>
          <p>المستمسكات والإجراءات الخاصة بإصدار وتأييد بطاقة السكن.</p>
        </div>
      </div>
    </section>

    <!-- Developer Info Section -->
    <section class="section-pad" id="developer">
      <div class="section-title">
        <h2>عن مطور المنصة</h2>
      </div>
      <div class="dev-container">
        <span class="dev-badge">DEVELOPER & PROGRAMMER</span>
        <div class="dev-details">
          <h3>MUSTAFA NEX</h3>
          <p>أنا مصطفى، مطور ومبرمج تطبيقات ومواقع إلكترونية، قمت بتطوير منصة وتطبيق «معاملتي» كدليل رقمي مستقل لخدمة المجتمع العراقي وتسهيل الوصول إلى تفاصيل المعاملات اليومية بكل وضوح وشفافية.</p>
          <a class="btn btn-gold" href="https://mustafanex.github.io/" target="_blank" rel="noopener">زيارة الموقع الشخصي ↗</a>
        </div>
      </div>
    </section>

    <!-- Support Section -->
    <section class="section-pad" id="support" style="background:var(--panel);">
      <div class="section-title">
        <h2>الدعم الفني والخدمة</h2>
        <p>إذا كان لديك أي استفسار أو واجهتك مشكلة فنية، تواصل معنا مباشرة</p>
      </div>
      <div class="support-container">
        <p style="color:var(--muted);margin:0;font-size:12px;">بريد الدعم الفني واستقبال المقترحات:</p>
        <div class="support-email">Hello.mustafanex@gmail.com</div>

        <form onsubmit="event.preventDefault(); alert('تم إرسال رسالتك بنجاح وسيتواصل معك فريق الدعم.');">
          <div class="form-group">
            <label>الاسم الكريم</label>
            <input type="text" placeholder="أدخل اسمك" required>
          </div>
          <div class="form-group">
            <label>عنوان البريد الإلكتروني</label>
            <input type="email" placeholder="email@example.com" required>
          </div>
          <div class="form-group">
            <label>تفاصيل الاستفسار أو المشكلة الفنية</label>
            <textarea rows="4" placeholder="اكتب استفسارك بالتفصيل..." required></textarea>
          </div>
          <button class="btn btn-gold" style="width:100%;margin-top:10px;" type="submit">إرسال إلى فريق الدعم الفني ✉</button>
        </form>
      </div>
    </section>
  </main>

  <footer class="footer">
    <div class="footer-disclaimer">
      تطبيق <b>معاملتي</b> هو دليل إرشادي رقمي مستقل يهدف إلى تسهيل وتبسيط الإجراءات للمواطنين، ولا يتبع أو يمثل أي جهة حكومية أو سياسية.
    </div>
    <div class="footer-copy">جميع الحقوق محفوظة منصة معاملتي © 2026</div>
  </footer>

  <!-- Store Modal -->
  <div class="modal" id="downloadModal">
    <div class="modal-card">
      <h3 style="font:600 20px Alexandria;color:var(--gold2);margin-top:0;">تنزيل التطبيق مجاناً</h3>
      <p style="font-size:12px;color:var(--muted);">اختر المتجر المناسب لهاتفك</p>
      <a class="store-btn" href="https://mustafanex.github.io/" target="_blank">
        <span style="font-size:20px;">🤖</span>
        <span>Google Play (Android)</span>
      </a>
      <a class="store-btn" href="https://mustafanex.github.io/" target="_blank">
        <span style="font-size:20px;">🍏</span>
        <span>App Store (iPhone)</span>
      </a>
      <button class="btn btn-outline" style="width:100%;margin-top:20px;" onclick="closeModal()">إغلاق</button>
    </div>
  </div>

  <script>
    function openModal(){ document.getElementById('downloadModal').classList.add('active'); }
    function closeModal(){ document.getElementById('downloadModal').classList.remove('active'); }
  </script>
</body>
</html>
