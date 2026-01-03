<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>The Digital Pulpit</title>
  <style>
    :root{
      --bg:#0b0f17;
      --card: rgba(255,255,255,.06);
      --border: rgba(255,255,255,.12);
      --text:#eaf0ff;
      --muted: rgba(234,240,255,.78);
      --accent:#ffffff;
    }
    *{box-sizing:border-box}
    body{margin:0;font-family:system-ui,-apple-system,Segoe UI,Roboto,Arial,sans-serif;background:var(--bg);color:var(--text)}
    .container{max-width:980px;margin:0 auto;padding:24px}
    header{position:sticky;top:0;background:rgba(11,15,23,.86);backdrop-filter: blur(10px);border-bottom:1px solid var(--border);z-index:10}
    .headRow{display:flex;justify-content:space-between;align-items:center;gap:16px}
    .brand{display:flex;gap:12px;align-items:center}
    .logo{width:38px;height:38px;border:1px solid var(--border);border-radius:12px;display:flex;align-items:center;justify-content:center;background:var(--card)}
    .name{font-weight:900}
    .tag{font-size:13px;color:var(--muted)}
    nav{display:flex;gap:14px;flex-wrap:wrap}
    nav a{color:var(--muted);text-decoration:none;font-weight:800}
    nav a.active{color:var(--text)}
    .card{background:var(--card);border:1px solid var(--border);border-radius:18px;padding:18px;margin-bottom:16px}
    .hero h1{margin:0 0 10px;font-size:34px;line-height:1.12}
    .muted{color:var(--muted)}
    .tiny{font-size:12px;color:var(--muted)}
    .grid{display:grid;gap:16px;grid-template-columns:1.1fr .9fr}
    @media(max-width:900px){.grid{grid-template-columns:1fr}}
    .btn{display:inline-block;background:var(--accent);color:#0b0f17;border:0;padding:11px 14px;border-radius:12px;font-weight:900;text-decoration:none;cursor:pointer}
    .btn.secondary{background:transparent;color:var(--text);border:1px solid var(--border)}
    .btn.full{width:100%}
    input,select{width:100%;padding:12px 12px;margin-top:6px;border-radius:12px;border:1px solid var(--border);background:rgba(0,0,0,.25);color:var(--text)}
    .cta{display:flex;gap:10px;flex-wrap:wrap;margin:12px 0}
    .verse{margin-top:10px;padding:12px;border-radius:14px;border:1px solid var(--border);background:rgba(0,0,0,.22)}
    .list{padding-left:18px;margin:10px 0}
    .pill{display:inline-block;padding:6px 10px;border-radius:999px;border:1px solid var(--border);background:rgba(255,255,255,.06);font-size:13px}
    .filters{display:grid;grid-template-columns:220px 1fr;gap:10px;margin-top:10px}
    @media(max-width:700px){.filters{grid-template-columns:1fr}}
    .list-grid{display:grid;gap:12px;grid-template-columns:repeat(2,1fr)}
    @media(max-width:900px){.list-grid{grid-template-columns:1fr}}
    .item{padding:14px;border-radius:16px;border:1px solid var(--border);background:rgba(0,0,0,.22)}
    .item a{color:var(--text);text-decoration:none;font-weight:900}
    .item .meta{display:flex;gap:10px;flex-wrap:wrap;margin-top:6px}
    .notice{margin-top:10px;min-height:20px}
    footer{border-top:1px solid var(--border);margin-top:20px}
    .footRow{display:flex;justify-content:space-between;gap:12px;flex-wrap:wrap}
    .ad-box{
      height:90px;border:1px dashed rgba(255,255,255,.25);
      border-radius:14px;display:flex;align-items:center;justify-content:center;background:rgba(0,0,0,.18)
    }
    .ad-label{font-size:12px;color:var(--muted);margin-bottom:8px}
    blockquote{margin:10px 0;padding:12px 14px;border-left:4px solid rgba(255,255,255,.25);background:rgba(0,0,0,.18);border-radius:12px}
    .toolbar{display:flex;gap:10px;flex-wrap:wrap;margin:12px 0}
    .metaRow{display:flex;gap:10px;flex-wrap:wrap;align-items:center}
    .hide{display:none !important;}
    a.link{color:var(--text)}
  </style>
</head>
<body>
  <header>
    <div class="container headRow">
      <div class="brand">
        <div class="logo">✝</div>
        <div>
          <div class="name" id="siteTitle">The Digital Pulpit</div>
          <div class="tag">KJV • The Blood of Christ • Salvation</div>
        </div>
      </div>
      <nav>
        <a href="#/home" id="navHome">Home</a>
        <a href="#/sermons" id="navSermons">Sermons</a>
        <a href="#/privacy" id="navPrivacy">Privacy</a>
      </nav>
    </div>
  </header>

  <main class="container">
    <!-- HOME -->
    <section id="viewHome" class="view">
      <section class="card hero">
        <h1>Preaching Christ. Proclaiming the Blood. Powered for This Generation.</h1>
        <p class="muted">
          No livestreams. Just Scripture-driven sermons delivered as text and audio (TTS),
          rooted in the <b>King James Bible</b> and centered on the Gospel of Jesus Christ.
        </p>
        <div class="cta">
          <a class="btn" href="#/sermons">Read Sermons</a>
          <a class="btn secondary" href="#/home#subscribe">Get Sermons by Email</a>
        </div>
        <div class="verse">
          “So then faith cometh by hearing, and hearing by the word of God.” — <b>Romans 10:17 (KJV)</b>
        </div>
      </section>

      <section class="grid">
        <div class="card">
          <h2>Service Schedule</h2>
          <ul class="list">
            <li><b>Sunday Morning</b> — Published 6:00 AM</li>
            <li><b>Sunday Evening</b> — Published 4:00 PM</li>
            <li><b>Wednesday Evening</b> — Published 4:00 PM</li>
          </ul>
          <p class="muted">Each sermon includes KJV Scripture, a clear Gospel invitation, and a “Listen” option.</p>
        </div>

        <div class="card" id="subscribe">
          <h2>Receive Every Sermon</h2>
          <p class="muted">Subscribe to receive each sermon by email. Unsubscribe anytime.</p>

          <form id="subscribeForm">
            <label class="muted" for="email">Email</label>
            <input id="email" name="email" type="email" placeholder="you@example.com" required />
            <button class="btn full" type="submit">Subscribe</button>
          </form>

          <div id="subscribeMsg" class="notice" aria-live="polite"></div>

          <p class="tiny muted">
            This ministry is supported by advertising so sermons remain freely available.
          </p>
          <p class="tiny muted">
            After you subscribe, you’ll receive a confirmation email. Click confirm to start receiving sermons.
          </p>
        </div>
      </section>

      <section class="card">
        <div class="ad-label">Advertisement</div>
        <div class="ad-box"><span class="muted">Ad Slot (place AdSense code here later)</span></div>
      </section>

      <section class="card">
        <h2>Statement</h2>
        <p>
          The Digital Pulpit is committed to the <b>King James Bible</b>, the saving power of the
          <b>Blood of Jesus Christ</b>, and salvation by grace through faith.
        </p>
        <p class="muted">Technology is our delivery method. Scripture is our authority.</p>
      </section>
    </section>

    <!-- SERMONS -->
    <section id="viewSermons" class="view hide">
      <section class="card">
        <h1>Sermons</h1>
        <p class="muted">Filter by service slot and open any sermon to read or listen.</p>

        <div class="filters">
          <select id="slotFilter">
            <option value="all">All services</option>
            <option value="Sunday Morning">Sunday Morning</option>
            <option value="Sunday Evening">Sunday Evening</option>
            <option value="Wednesday Evening">Wednesday Evening</option>
          </select>
          <input id="search" type="search" placeholder="Search title or scripture..." />
        </div>
      </section>

      <section class="card">
        <div class="ad-label">Advertisement</div>
        <div class="ad-box"><span class="muted">Ad Slot</span></div>
      </section>

      <section id="sermonList" class="list-grid"></section>
    </section>

    <!-- SERMON DETAIL -->
    <section id="viewSermon" class="view hide">
      <article class="card sermon">
        <div class="metaRow">
          <span id="sermonSlot" class="pill"></span>
          <span id="sermonDate" class="muted"></span>
        </div>

        <h1 id="sermonTitle"></h1>

        <div class="toolbar">
          <button id="speakBtn" class="btn">Listen (TTS)</button>
          <button id="stopBtn" class="btn secondary">Stop</button>
          <a class="btn secondary" href="#/sermons">Back to Sermons</a>
          <a class="btn secondary" id="openBackendLink" href="#" target="_blank" rel="noopener">Open on Web App</a>
        </div>

        <section>
          <div class="ad-label">Advertisement</div>
          <div class="ad-box"><span class="muted">Ad Slot</span></div>
        </section>

        <h2>Primary Text (KJV)</h2>
        <blockquote id="sermonPrimary"></blockquote>

        <h2>Opening Prayer</h2>
        <p id="sermonOpeningPrayer"></p>

        <h2>Sermon</h2>
        <div id="sermonBody"></div>

        <section style="margin:14px 0">
          <div class="ad-label">Advertisement</div>
          <div class="ad-box"><span class="muted">Ad Slot</span></div>
        </section>

        <h2>The Gospel & The Blood (KJV)</h2>
        <div id="sermonGospel"></div>

        <h2>How to Be Saved</h2>
        <div id="sermonSalvation"></div>

        <h2>Closing Prayer</h2>
        <p id="sermonClosingPrayer"></p>

        <h2>Reflection Questions</h2>
        <ul id="sermonQuestions"></ul>

        <p class="tiny muted">
          Note: Sermons are produced using Scripture-driven tools and reviewed for faithfulness to the KJV and the Gospel.
        </p>
      </article>
    </section>

    <!-- PRIVACY -->
    <section id="viewPrivacy" class="view hide">
      <section class="card">
        <h1>Privacy</h1>
        <p>We collect email addresses only to deliver sermons and ministry updates.</p>
        <ul class="list">
          <li>You may unsubscribe at any time.</li>
          <li>We do not sell your email address.</li>
          <li>Advertising may use cookies/identifiers depending on your ad provider.</li>
        </ul>
        <p class="tiny muted">
          If you enable AdSense later, add their required disclosures and cookie consent notice if needed.
        </p>
      </section>
    </section>
  </main>

  <footer>
    <div class="container footRow">
      <span class="muted">© <span id="year"></span> The Digital Pulpit</span>
      <span class="muted">KJV • Gospel • Salvation</span>
    </div>
  </footer>

  <script>
    /*************************************************************
     * CONFIG — IMPORTANT
     * Replace with your Google Apps Script Web App URL.
     * Example:
     * const BACKEND_WEBAPP_URL = "https://script.google.com/macros/s/AKfycb.../exec";
     *************************************************************/
    const BACKEND_WEBAPP_URL = "PASTE_YOUR_APPS_SCRIPT_WEBAPP_URL_HERE";

    // Sermons stored on the frontend (easy to maintain for MVP)
    // IDs should match what your backend emails link to (page=sermon&id=...)
    const SERMONS = [
      {
        id: "2026-01-04-sun-am-power-of-the-blood",
        date: "2026-01-04",
        serviceSlot: "Sunday Morning",
        title: "The Power of the Blood",
        primaryRef: "Revelation 1:5 (KJV)",
        primaryText: "Unto him that loved us, and washed us from our sins in his own blood.",
        summary: "A KJV sermon on the necessity and saving power of Christ’s blood and the Gospel invitation.",
        openingPrayer:
          "Heavenly Father, we thank Thee for Thy Word and the precious Blood of Jesus Christ. Open our hearts to truth, convict the lost, strengthen the saved, and glorify Thy Son. In Jesus’ name, Amen.",
        body: [
          "From Genesis to Revelation, the Bible is a book of blood. Modern religion avoids the subject, but the Bible never does. Without the Blood of Jesus Christ, there is no forgiveness, no cleansing, and no salvation.",
          "Hebrews 9:22 says, “and without shedding of blood is no remission.” Sin demands payment. God is holy. Man is guilty. No good works or religion can wash away sin—only blood.",
          "1 Peter 1:18–19 calls it “the precious blood of Christ.” Jesus was sinless. He paid a debt He did not owe for sinners who could never pay it.",
          "1 John 1:7 says the blood of Jesus Christ cleanseth us from all sin. Romans 5:9 declares we are justified by his blood. Colossians 1:20 says peace is made through the blood of his cross."
        ],
        gospel: [
          "1 Corinthians 15:1–4 (KJV): Christ died for our sins… He was buried… and He rose again the third day.",
          "Salvation is not earned. Salvation is received by faith in the finished work of Jesus Christ."
        ],
        salvation: [
          "Romans 10:9–10 (KJV): That if thou shalt confess with thy mouth the Lord Jesus, and shalt believe in thine heart that God hath raised him from the dead, thou shalt be saved.",
          "Romans 10:13 (KJV): For whosoever shall call upon the name of the Lord shall be saved."
        ],
        closingPrayer:
          "Lord, thank You for the Blood that was shed for sinners. Draw souls unto Thyself, strengthen believers, and help us never be ashamed of the Gospel. In Jesus’ name, Amen.",
        questions: [
          "Have you trusted fully in the Blood of Christ for salvation?",
          "Are you resting in grace—or still trying to earn forgiveness?",
          "How does knowing the price Christ paid change how you live?"
        ]
      },
      {
        id: "2026-01-04-sun-pm-come-unto-me",
        date: "2026-01-04",
        serviceSlot: "Sunday Evening",
        title: "Come Unto Me",
        primaryRef: "Matthew 11:28 (KJV)",
        primaryText: "Come unto me, all ye that labour and are heavy laden, and I will give you rest.",
        summary: "A KJV sermon calling the weary to Christ, pointing to the cross, the Blood, and salvation by faith.",
        openingPrayer:
          "Father in heaven, we come to Thee in Jesus’ name. Speak to every heart through Thy Word. Draw the lost to Christ, strengthen the saved, and let the Name of Jesus be lifted up. Amen.",
        body: [
          "This world is full of weary souls. Many are tired of trying, tired of failing, tired of sin, and tired of the emptiness. Yet Jesus Christ gives a call that religion cannot give. He does not say, “Try harder.” He says, “Come unto me.”",
          "Christ invites the burdened—those who labour under guilt, fear, shame, and the weight of sin. Sin is not a light thing. It presses the conscience. It steals peace. It brings separation from God. And no man can carry it away by his own works.",
          "Jesus says, “and I will give you rest.” That rest is not found in turning over a new leaf. It is found in a finished work. When Jesus died on the cross, He paid the debt. When He rose again, He proved the payment was accepted.",
          "Hebrews 9:22 (KJV) says, “without shedding of blood is no remission.” Remission requires blood. And the Blood that saves is the Blood of Jesus Christ.",
          "Romans 5:9 (KJV) says we are “justified by his blood.” 1 John 1:7 (KJV) says “the blood of Jesus Christ his Son cleanseth us from all sin.” If you will come to Christ by faith, He offers cleansing, pardon, and peace with God.",
          "To come unto Christ is to lay down the hope of saving yourself and to trust Him wholly—believing the Gospel: that Christ died for your sins, was buried, and rose again."
        ],
        gospel: [
          "1 Corinthians 15:1–4 (KJV): Christ died for our sins… He was buried… and He rose again the third day.",
          "Revelation 1:5 (KJV): “…washed us from our sins in his own blood.”"
        ],
        salvation: [
          "Ephesians 2:8–9 (KJV): “For by grace are ye saved through faith… not of works…”",
          "Romans 10:13 (KJV): “For whosoever shall call upon the name of the Lord shall be saved.”"
        ],
        closingPrayer:
          "Lord Jesus, thank You for calling the weary to Yourself. Thank You for Thy precious Blood that cleanseth from all sin. Save the lost, strengthen the saved, and give rest to every burdened heart that comes to Thee by faith. Amen.",
        questions: [
          "What burden are you carrying that Christ is calling you to bring to Him?",
          "Have you truly come to Christ by faith, or are you still trying to earn peace by works?",
          "Do you believe Jesus’ Blood is sufficient to cleanse you from all sin?"
        ]
      },
      {
        id: "2026-01-08-wed-pm-the-just-shall-live-by-faith",
        date: "2026-01-08",
        serviceSlot: "Wednesday Evening",
        title: "The Just Shall Live by Faith",
        primaryRef: "Romans 1:17 (KJV)",
        primaryText: "The just shall live by faith.",
        summary: "A KJV teaching sermon on saving faith, assurance in Christ’s Blood, and living the Christian life by faith.",
        openingPrayer:
          "Lord, open Thy Word to us tonight. Teach us to rest in Christ, to trust the Gospel, and to live by faith. Let every soul be pointed to the cross and the Blood of Jesus. In Jesus’ name, Amen.",
        body: [
          "God does not call us to a life built on feelings, trends, or human strength. The Christian life begins by faith and continues by faith. The Scripture says plainly: “The just shall live by faith.”",
          "How does a man become “just”? Not by works. We are sinners. But God justifies sinners through Jesus Christ. Romans 5:9 (KJV) says, “Being now justified by his blood, we shall be saved from wrath through him.”",
          "Saving faith is trusting the finished work of Christ—His death, burial, and resurrection—and trusting His Blood as the payment for your sins.",
          "Hebrews 9:22 (KJV) says remission comes only by blood. 1 John 1:7 (KJV) says His Blood cleanseth us from all sin. Forgiveness is granted because Christ shed His Blood.",
          "Assurance is not found in how strong your faith feels, but in how sufficient Christ is. The object of faith matters: Jesus Christ and His Blood.",
          "After salvation, we still live by faith—believing God’s promises, obeying His Word, and walking with Him daily. Faith clings to Scripture when the world mocks truth.",
          "If you are not saved, tonight is the night to come to Christ. The price has been paid. The Blood has been shed. The Gospel has been preached. Will you believe?"
        ],
        gospel: [
          "1 Corinthians 15:1–4 (KJV): Christ died for our sins… He was buried… and He rose again the third day.",
          "Ephesians 2:8–9 (KJV): Salvation is by grace through faith, not of works.",
          "Romans 5:9 (KJV): We are justified by His Blood."
        ],
        salvation: [
          "Romans 10:9–10 (KJV): Believe in thine heart… and thou shalt be saved.",
          "Romans 10:13 (KJV): “For whosoever shall call upon the name of the Lord shall be saved.”"
        ],
        closingPrayer:
          "Father, thank You for the Gospel and for the Blood of Jesus Christ. Give assurance to the saved, and save the lost. Teach us to live by faith, anchored in Thy Word. In Jesus’ name, Amen.",
        questions: [
          "Are you trusting Christ alone for salvation, or are you mixing faith with works?",
          "Where do you look for assurance—your feelings or Christ’s finished work?",
          "What area of your life needs to be brought under faith and obedience to God’s Word?"
        ]
      }
    ];

    // ===== Utilities =====
    const $ = (id) => document.getElementById(id);
    const escapeHtml = (str) => String(str||"")
      .replaceAll("&","&amp;").replaceAll("<","&lt;").replaceAll(">","&gt;")
      .replaceAll('"',"&quot;").replaceAll("'","&#039;");

    function setActiveNav(route){
      $("navHome").classList.toggle("active", route.startsWith("#/home"));
      $("navSermons").classList.toggle("active", route.startsWith("#/sermons") || route.startsWith("#/sermon"));
      $("navPrivacy").classList.toggle("active", route.startsWith("#/privacy"));
    }

    function showView(viewId){
      for (const el of document.querySelectorAll(".view")) el.classList.add("hide");
      $(viewId).classList.remove("hide");
    }

    function renderSermonList(){
      const list = $("sermonList");
      const slot = $("slotFilter").value;
      const q = ($("search").value || "").toLowerCase();

      const filtered = SERMONS
        .filter(s => slot === "all" ? true : s.serviceSlot === slot)
        .filter(s => !q ? true : (s.title + " " + s.primaryRef).toLowerCase().includes(q))
        .sort((a,b) => String(b.date||"").localeCompare(String(a.date||"")));

      list.innerHTML = filtered.map(s => `
        <div class="item">
          <a href="#/sermon/${encodeURIComponent(s.id)}">${escapeHtml(s.title)}</a>
          <div class="meta">
            <span class="pill">${escapeHtml(s.serviceSlot)}</span>
            <span class="muted">${escapeHtml(s.date)}</span>
            <span class="muted">${escapeHtml(s.primaryRef)}</span>
          </div>
          <div class="muted tiny">${escapeHtml(s.summary||"")}</div>
        </div>
      `).join("");
    }

    function renderSermon(id){
      const s = SERMONS.find(x => x.id === id);
      if (!s){
        $("viewSermon").innerHTML = `<section class="card"><h1>Sermon not found.</h1><a class="link" href="#/sermons">Back</a></section>`;
        return;
      }

      $("sermonSlot").textContent = s.serviceSlot;
      $("sermonDate").textContent = s.date;
      $("sermonTitle").textContent = s.title;

      $("sermonPrimary").innerHTML = `<b>${escapeHtml(s.primaryRef)}</b><br>${escapeHtml(s.primaryText)}`;
      $("sermonOpeningPrayer").textContent = s.openingPrayer;

      $("sermonBody").innerHTML = (s.body||[]).map(p => `<p>${escapeHtml(p)}</p>`).join("");
      $("sermonGospel").innerHTML = (s.gospel||[]).map(p => `<p>${escapeHtml(p)}</p>`).join("");
      $("sermonSalvation").innerHTML = (s.salvation||[]).map(p => `<p>${escapeHtml(p)}</p>`).join("");

      $("sermonClosingPrayer").textContent = s.closingPrayer;
      $("sermonQuestions").innerHTML = (s.questions||[]).map(q => `<li>${escapeHtml(q)}</li>`).join("");

      // Link to backend-hosted sermon page (optional, but helpful)
      if (BACKEND_WEBAPP_URL && BACKEND_WEBAPP_URL.startsWith("http")) {
        $("openBackendLink").href = `${BACKEND_WEBAPP_URL}?page=sermon&id=${encodeURIComponent(s.id)}`;
      } else {
        $("openBackendLink").classList.add("hide");
      }
    }

    // ===== TTS (Text-to-Speech) =====
    function getTextForTTS(){
      const el = document.querySelector(".sermon");
      if (!el) return "";
      const clone = el.cloneNode(true);
      // remove ad labels/boxes if present in future
      clone.querySelectorAll(".ad-box, .ad-label").forEach(n => n.remove());
      return clone.innerText.replace(/\s+/g, " ").trim();
    }

    function ttsSpeak(){
      if (!("speechSynthesis" in window)) {
        alert("Text-to-Speech is not supported on this device/browser.");
        return;
      }
      window.speechSynthesis.cancel();
      const text = getTextForTTS();
      if (!text) return;

      const u = new SpeechSynthesisUtterance(text);
      u.rate = 1.0; u.pitch = 1.0; u.volume = 1.0;
      window.speechSynthesis.speak(u);
    }

    function ttsStop(){
      if ("speechSynthesis" in window) window.speechSynthesis.cancel();
    }

    // ===== Subscribe (operational) =====
    async function subscribe(email){
      if (!BACKEND_WEBAPP_URL || !BACKEND_WEBAPP_URL.startsWith("http")) {
        throw new Error("Backend Web App URL is not set. Paste your Apps Script Web App URL into BACKEND_WEBAPP_URL.");
      }

      const res = await fetch(`${BACKEND_WEBAPP_URL}?path=subscribe`, {
        method: "POST",
        headers: {"Content-Type":"application/json"},
        body: JSON.stringify({ email })
      });

      const data = await res.json().catch(() => ({}));
      if (!data.ok) throw new Error(data.error || "Subscribe failed.");
      return data.message || "Confirmation email sent.";
    }

    function wireSubscribe(){
      const form = $("subscribeForm");
      const msg = $("subscribeMsg");
      form.addEventListener("submit", async (e) => {
        e.preventDefault();
        msg.textContent = "";
        const email = $("email").value.trim();

        try{
          msg.textContent = "Submitting…";
          const m = await subscribe(email);
          msg.textContent = m;
        } catch(err){
          msg.textContent = "Error: " + err.message;
        }
      });
    }

    function wireSermonControls(){
      $("speakBtn").addEventListener("click", ttsSpeak);
      $("stopBtn").addEventListener("click", ttsStop);
    }

    // ===== Router =====
    function route(){
      const hash = window.location.hash || "#/home";
      setActiveNav(hash);

      // home anchor for subscribe
      if (hash.startsWith("#/home")){
        showView("viewHome");
        // scroll to subscribe if second hash section
        if (hash.includes("#subscribe")) {
          setTimeout(() => document.getElementById("subscribe")?.scrollIntoView({behavior:"smooth"}), 50);
        }
        return;
      }

      if (hash.startsWith("#/sermons")){
        showView("viewSermons");
        renderSermonList();
        return;
      }

      if (hash.startsWith("#/sermon/")){
        const id = decodeURIComponent(hash.replace("#/sermon/",""));
        showView("viewSermon");
        renderSermon(id);
        return;
      }

      if (hash.startsWith("#/privacy")){
        showView("viewPrivacy");
        return;
      }

      // default
      window.location.hash = "#/home";
    }

    function init(){
      $("year").textContent = new Date().getFullYear();

      // filters
      $("slotFilter").addEventListener("change", renderSermonList);
      $("search").addEventListener("input", renderSermonList);

      wireSubscribe();
      wireSermonControls();

      window.addEventListener("hashchange", route);
      route();
    }

    init();
  </script>
</body>
</html>
