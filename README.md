
<style>
@import url('https://fonts.googleapis.com/css2?family=Fira+Code:wght@400;600;700&display=swap');
*{box-sizing:border-box;margin:0;padding:0;}
.wrap{background:#000;border-radius:12px;overflow:hidden;color:#00ff41;font-family:'Fira Code',monospace;font-size:12px;position:relative;}
#mc{position:absolute;top:0;left:0;width:100%;height:100%;opacity:.12;pointer-events:none;z-index:0;}
.content{position:relative;z-index:1;}
.wave{height:4px;background:linear-gradient(90deg,#008f11,#00ff41,#39ff14,#00ff41,#008f11);background-size:300% 100%;animation:sh 3s linear infinite;}
@keyframes sh{0%{background-position:0%}100%{background-position:300%}}
/* HEADER */
.header{background:linear-gradient(180deg,#000 0%,#001200 70%,#002200 100%);padding:26px 20px 18px;text-align:center;border-bottom:2px solid #00ff4130;}
.hname{font-size:28px;font-weight:700;color:#00ff41;text-shadow:0 0 25px #00ff41,0 0 50px #00ff4160;letter-spacing:3px;margin-bottom:4px;}
.hrole{font-size:12px;color:#39ff14;letter-spacing:2px;margin-bottom:4px;text-shadow:0 0 10px #39ff14;}
.hsubrole{font-size:10px;color:#006600;letter-spacing:1px;margin-bottom:14px;}
.typing-line{font-size:11px;color:#00ff41;height:17px;margin-bottom:14px;text-shadow:0 0 8px #00ff41;}
.cur{border-right:2px solid #00ff41;animation:blink .7s step-end infinite;}
@keyframes blink{50%{border-color:transparent}}
.social-row{display:flex;justify-content:center;gap:6px;flex-wrap:wrap;margin-bottom:10px;}
.sb{padding:4px 12px;border-radius:3px;font-size:9px;font-weight:700;letter-spacing:.7px;border:1px solid #00ff41;background:#001200;color:#00ff41;text-shadow:0 0 6px #00ff41;}
.views{font-size:9px;color:#004400;letter-spacing:1.5px;}
.pulse{display:inline-block;width:6px;height:6px;border-radius:50%;background:#00ff41;margin-right:5px;animation:p 1.5s ease infinite;box-shadow:0 0 5px #00ff41;}
@keyframes p{0%,100%{opacity:1;transform:scale(1)}50%{opacity:.2;transform:scale(1.8)}}

/* GIF SECTION */
.gif-section{padding:14px 20px;border-bottom:1px solid #00ff4115;text-align:center;}
.gif-box{display:inline-block;border:1px solid #00ff4140;border-radius:8px;padding:8px 16px;background:#001200;color:#004400;font-size:9px;letter-spacing:1px;}
.gif-icon{font-size:42px;display:block;margin-bottom:4px;filter:drop-shadow(0 0 10px #00ff41);}

/* SECTION */
.section{padding:14px 18px;border-bottom:1px solid #00ff4112;}
.stitle{font-size:12px;font-weight:700;color:#00ff41;margin-bottom:10px;text-shadow:0 0 8px #00ff4160;letter-spacing:.5px;}
.stitle span{color:#004400;margin-right:3px;}

/* TERMINAL */
.term{background:#020d02;border:1px solid #00ff4135;border-radius:6px;padding:11px 13px;font-size:9.5px;line-height:2;color:#006600;overflow:auto;}
.k{color:#00ff41;font-weight:700;text-shadow:0 0 6px #00ff41;}
.v{color:#39ff14;}.hi{color:#7fff7f;}.dim{color:#003300;}

/* BACKEND HERO CARD */
.be-hero{background:linear-gradient(135deg,#001a00,#002a00);border:1px solid #00ff4150;border-radius:8px;padding:12px 14px;position:relative;overflow:hidden;margin-bottom:10px;}
.be-hero::before{content:'';position:absolute;top:0;left:0;right:0;height:3px;background:linear-gradient(90deg,#00ff41,#39ff14,#7fff00,#39ff14,#00ff41);background-size:200% 100%;animation:sh 2s linear infinite;}
.be-hero-title{font-size:10px;font-weight:700;color:#00ff41;text-shadow:0 0 10px #00ff41;letter-spacing:1.5px;margin-bottom:8px;text-transform:uppercase;}
.be-pills{display:flex;flex-wrap:wrap;gap:5px;}
.pill{padding:4px 9px;border-radius:3px;font-size:9.5px;font-weight:700;border:1px solid #00ff4160;background:#001200;color:#00ff41;letter-spacing:.3px;}
.pill.secondary{border-color:#39ff1440;color:#39ff14;}
.pill.dim-pill{border-color:#00440040;color:#006600;}

/* TECH GRID */
.tech-grid{display:grid;grid-template-columns:1fr 1fr;gap:7px;}
.tc{background:#020d02;border:1px solid #00ff4122;border-radius:6px;padding:9px 11px;position:relative;overflow:hidden;}
.tc::before{content:'';position:absolute;top:0;left:0;right:0;height:1.5px;background:linear-gradient(90deg,#00ff41,#39ff14);}
.tc-t{font-size:8.5px;text-transform:uppercase;letter-spacing:.7px;color:#004400;margin-bottom:7px;font-weight:700;}
.pills{display:flex;flex-wrap:wrap;gap:4px;}
.ai-tc{border-color:#39ff1445;grid-column:span 2;}
.ai-tc::before{background:linear-gradient(90deg,#00ff41,#39ff14,#7fff00,#39ff14,#00ff41);background-size:200% 100%;animation:sh 2.5s linear infinite;}

/* DB */
.db-grid{display:grid;grid-template-columns:1fr 1fr;gap:7px;}
.db-c{background:#020d02;border-radius:6px;padding:10px 11px;position:relative;overflow:hidden;}
.rel-c{border:1px solid #00ff4135;}.rel-c::before{content:'';position:absolute;top:0;left:0;right:0;height:2px;background:linear-gradient(90deg,#00ff41,#39ff14,#00cc33);}
.norel-c{border:1px solid #39ff1430;}.norel-c::before{content:'';position:absolute;top:0;left:0;right:0;height:2px;background:linear-gradient(90deg,#39ff14,#7fff00,#00ff41);}
.db-sub{font-size:8.5px;text-transform:uppercase;letter-spacing:.7px;color:#004400;margin-bottom:7px;font-weight:700;}
.db-i{display:flex;align-items:center;gap:6px;padding:3px 0;border-bottom:1px solid #00ff4108;}
.db-d{width:7px;height:7px;border-radius:50%;box-shadow:0 0 4px currentColor;flex-shrink:0;}
.db-n{font-size:9.5px;color:#39ff14;flex:1;}
.db-tp{font-size:7.5px;padding:1px 5px;border-radius:10px;border:1px solid #00ff4130;color:#004400;}

/* CERTS */
.cert-list{display:flex;flex-direction:column;gap:6px;}
.cert-i{display:flex;align-items:center;gap:9px;background:#020d02;border:1px solid #00ff4128;border-radius:6px;padding:8px 11px;position:relative;overflow:hidden;}
.cert-i::before{content:'';position:absolute;left:0;top:0;bottom:0;width:2px;background:#00ff41;box-shadow:0 0 6px #00ff41;}
.ci-icon{font-size:16px;}
.ci-name{font-size:10.5px;font-weight:700;color:#00ff41;}
.ci-sub{font-size:8.5px;color:#004400;margin-top:2px;}
.ci-tag{margin-left:auto;padding:2px 7px;border-radius:2px;font-size:7.5px;font-weight:700;letter-spacing:.5px;border:1px solid #00ff4150;color:#39ff14;background:#001200;white-space:nowrap;}

/* STATS */
.stats-row{display:grid;grid-template-columns:repeat(3,1fr);gap:7px;}
.stat{background:#020d02;border:1px solid #00ff4125;border-radius:6px;padding:10px;text-align:center;position:relative;overflow:hidden;}
.stat::before{content:'';position:absolute;top:0;left:0;right:0;height:1.5px;background:#00ff41;}
.sv{font-size:20px;font-weight:700;color:#00ff41;text-shadow:0 0 12px #00ff41;}
.sl{font-size:7.5px;text-transform:uppercase;letter-spacing:.6px;color:#004400;margin-top:3px;}

/* FOOTER GIF */
.footer-gif{padding:14px 20px 10px;text-align:center;border-top:1px solid #00ff4115;}
.footer-msg{text-align:center;padding:8px 20px 12px;color:#003300;font-size:9.5px;letter-spacing:.5px;}
.footer-msg span{color:#00ff41;}
</style>

<div class="wrap">
<canvas id="mc"></canvas>
<div class="content">
  <div class="wave"></div>

  <!-- HEADER -->
  <div class="header">
    <div class="hname">Edwar Ramírez</div>
    <div class="hrole">> _ BACKEND DEVELOPER</div>
    <div class="hsubrole">Java · Spring Boot · Microservices · REST APIs</div>
    <div class="typing-line"><span class="cur" id="t"></span></div>
    <div class="social-row">
      <span class="sb">LinkedIn</span>
      <span class="sb">Twitter</span>
      <span class="sb">StackOverflow</span>
      <span class="sb">Gmail</span>
    </div>
    <div class="views"><span class="pulse"></span>SYSTEM ACCESS COUNT :: 417</div>
  </div>

  <!-- GIF 1 - HEADER GIF centered -->
  <div class="gif-section">
    <div class="gif-box">
      <span class="gif-icon">🖥️</span>
      GIF · Programador en terminal (i.pinimg.com)
    </div>
  </div>

  <!-- ABOUT -->
  <div class="section">
    <div class="stitle"><span>></span> whoami</div>
    <div class="term">
      <span class="dim">╔══════════════════════════════════════════╗</span><br>
      <span class="dim">║</span> <span class="k">USER</span>    :: <span class="v">Edwar Ramírez</span><br>
      <span class="dim">║</span> <span class="k">NODE</span>    :: <span class="v">Guayaquil, Ecuador 🇪🇨</span><br>
      <span class="dim">║</span> <span class="k">ROLE</span>    :: <span class="hi">Backend Developer [PRIMARY]</span><br>
      <span class="dim">║</span> <span class="k">FACULTY</span> :: <span class="v">UTEG · Software Engineering</span><br>
      <span class="dim">║</span> <span class="k">STATUS</span>  :: <span class="hi">ACTIVE · open_to_collaborate</span><br>
      <span class="dim">╠══════════════════════════════════════════╣</span><br>
      <span class="dim">║</span> <span class="k">CERTS</span>:<br>
      <span class="dim">║</span>&nbsp;&nbsp;<span class="v">[★] Deep Learning Specialization</span><br>
      <span class="dim">║</span>&nbsp;&nbsp;<span class="v">[★] Artium Certified Developer</span><br>
      <span class="dim">╠══════════════════════════════════════════╣</span><br>
      <span class="dim">║</span> <span class="k">CONTACT</span> :: <span class="v">edwarddelcastillo4@gmail.com</span><br>
      <span class="dim">╚══════════════════════════════════════════╝</span>
    </div>
  </div>

  <!-- TECH STACK -->
  <div class="section">
    <div class="stitle"><span>></span> ls ./tech-stack</div>

    <!-- BACKEND HERO -->
    <div class="be-hero">
      <div class="be-hero-title">⚙️ Backend [PRIMARY FOCUS]</div>
      <div class="be-pills">
        <span class="pill">☕ Java</span>
        <span class="pill">🌿 Spring Boot</span>
        <span class="pill">🌱 Spring Framework</span>
        <span class="pill">📄 JSP</span>
        <span class="pill">🔗 REST API</span>
        <span class="pill">🧩 Microservices</span>
        <span class="pill">🐍 Python</span>
      </div>
    </div>

    <div class="tech-grid">
      <div class="tc">
        <div class="tc-t">// Frontend</div>
        <div class="pills">
          <span class="pill secondary">🔺 Angular</span>
          <span class="pill secondary">🧡 HTML5</span>
          <span class="pill secondary">💙 CSS3</span>
        </div>
      </div>
      <div class="tc">
        <div class="tc-t">// DevOps & Tools</div>
        <div class="pills">
          <span class="pill secondary">🐋 Docker</span>
          <span class="pill secondary">🔀 Git</span>
          <span class="pill secondary">🐙 GitHub</span>
        </div>
      </div>
      <div class="tc ai-tc">
        <div class="tc-t" style="color:#39ff14;">// 🤖 AI & Deep Learning [CERTIFIED]</div>
        <div class="pills">
          <span class="pill">🔥 TensorFlow</span>
          <span class="pill">🔴 Keras</span>
          <span class="pill">📐 NumPy</span>
          <span class="pill">🐼 Pandas</span>
        </div>
      </div>
      <div class="tc">
        <div class="tc-t">// Hardware & IoT</div>
        <div class="pills">
          <span class="pill dim-pill">⚡ Arduino</span>
          <span class="pill dim-pill">🍓 Raspberry Pi</span>
        </div>
      </div>
    </div>
  </div>

  <!-- DATABASES -->
  <div class="section">
    <div class="stitle"><span>></span> ls ./databases</div>
    <div class="db-grid">
      <div class="db-c rel-c">
        <div class="db-sub">🔗 Relational · SQL</div>
        <div class="db-i"><div class="db-d" style="background:#00ff41;color:#00ff41;"></div><span class="db-n">MySQL</span><span class="db-tp">SQL</span></div>
        <div class="db-i"><div class="db-d" style="background:#39ff14;color:#39ff14;"></div><span class="db-n">PostgreSQL</span><span class="db-tp">SQL</span></div>
        <div class="db-i"><div class="db-d" style="background:#00cc33;color:#00cc33;"></div><span class="db-n">Oracle DB</span><span class="db-tp">SQL</span></div>
        <div class="db-i"><div class="db-d" style="background:#008f11;color:#008f11;"></div><span class="db-n">SQLite</span><span class="db-tp">SQL</span></div>
        <div class="db-i"><div class="db-d" style="background:#005c00;color:#005c00;"></div><span class="db-n">SQL Server</span><span class="db-tp">SQL</span></div>
      </div>
      <div class="db-c norel-c">
        <div class="db-sub">🍃 Non-Relational · NoSQL</div>
        <div class="db-i"><div class="db-d" style="background:#00ff41;color:#00ff41;"></div><span class="db-n">MongoDB</span><span class="db-tp">Document</span></div>
        <div class="db-i"><div class="db-d" style="background:#39ff14;color:#39ff14;"></div><span class="db-n">Redis</span><span class="db-tp">Key-Value</span></div>
        <div class="db-i"><div class="db-d" style="background:#00cc33;color:#00cc33;"></div><span class="db-n">Firebase</span><span class="db-tp">Document</span></div>
        <div class="db-i"><div class="db-d" style="background:#008f11;color:#008f11;"></div><span class="db-n">Cassandra</span><span class="db-tp">Wide-Col</span></div>
      </div>
    </div>
  </div>

  <!-- CERTS -->
  <div class="section">
    <div class="stitle"><span>></span> cat ./certifications.log</div>
    <div class="cert-list">
      <div class="cert-i"><span class="ci-icon">🧠</span><div><div class="ci-name">Deep Learning Specialization</div><div class="ci-sub">Coursera / deeplearning.ai · Neural Networks, CNN, RNN</div></div><span class="ci-tag">VERIFIED</span></div>
      <div class="cert-i"><span class="ci-icon">🤖</span><div><div class="ci-name">Artium Certified Developer</div><div class="ci-sub">Artium · Software Development Best Practices</div></div><span class="ci-tag">VERIFIED</span></div>
      <div class="cert-i"><span class="ci-icon">🏆</span><div><div class="ci-name">Tech Competitions & Events</div><div class="ci-sub">UTEG University · Recognitions & Awards</div></div><span class="ci-tag">AWARDED</span></div>
    </div>
  </div>

  <!-- STATS -->
  <div class="section">
    <div class="stitle"><span>></span> git log --stats</div>
    <div class="stats-row">
      <div class="stat"><div class="sv">131</div><div class="sl">Contributions</div></div>
      <div class="stat"><div class="sv">3</div><div class="sl">Longest Streak</div></div>
      <div class="stat"><div class="sv" style="font-size:14px;">OPEN</div><div class="sl">To Collaborate</div></div>
    </div>
  </div>

  <!-- GIF 2 - FOOTER GIF -->
  <div class="footer-gif">
    <div class="gif-box">
      <span class="gif-icon">🌆</span>
      GIF · Ciudad cyberpunk (i.redd.it)
    </div>
  </div>

  <div class="footer-msg">
    <span>> There is no spoon. Only clean code. &nbsp;&nbsp;[ SYSTEM SHUTDOWN... ]</span>
  </div>
  <div class="wave" style="animation-direction:reverse;"></div>
</div>
</div>

<script>
/* Matrix rain */
const canvas=document.getElementById('mc');
const ctx=canvas.getContext('2d');
function resize(){const p=canvas.parentElement;canvas.width=p.offsetWidth;canvas.height=p.offsetHeight;}
resize();
const chars='アイウエオカキクケコサシスセソタチツテトナニヌネノ01アカサタナハマ0110ヤラワ';
const fs=11;let cols,drops;
function init(){cols=Math.floor(canvas.width/fs);drops=Array(cols).fill(1);}
init();
function draw(){
  ctx.fillStyle='rgba(0,0,0,0.06)';ctx.fillRect(0,0,canvas.width,canvas.height);
  ctx.font=fs+'px Fira Code';
  for(let i=0;i<drops.length;i++){
    const c=chars[Math.floor(Math.random()*chars.length)];
    ctx.fillStyle=drops[i]*fs<25?'#7fff7f':'#00ff41';
    ctx.fillText(c,i*fs,drops[i]*fs);
    if(drops[i]*fs>canvas.height&&Math.random()>.975)drops[i]=0;
    drops[i]++;
  }
}
setInterval(draw,50);

/* Typing */
const ph=[
  '> Backend Developer | Java | Spring Boot...',
  '> Microservices & REST APIs ready...',
  '> Deep Learning modules active...',
  '> Arduino | Raspberry Pi | IoT online...',
  '> Wake up, Neo... 🟢'
];
let pi=0,ci=0,del=false;
const el=document.getElementById('t');
function type(){
  const p=ph[pi];
  if(!del){el.textContent=p.slice(0,++ci);if(ci===p.length){del=true;setTimeout(type,1800);return;}}
  else{el.textContent=p.slice(0,--ci);if(ci===0){del=false;pi=(pi+1)%ph.length;}}
  setTimeout(type,del?28:60);
}
type();
</script>

