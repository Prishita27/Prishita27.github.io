# Prishita27.github.io
This is my Github pages site
 (cd "$(git rev-parse --show-toplevel)" && printf '%s' 'diff --git a/index.html b/index.html
index 5baaaa69bd26094463db0edf5d11d57d90080ef0..0b4fbcd83870b447c2118eb6cc8712a86a1971d0 100644
--- a/index.html
+++ b/index.html
@@ -1,472 +1,84 @@
-<!DOCTYPE html>
+<!doctype html>
 <html lang="en">
 <head>
-<meta charset="UTF-8">
-<title>NEON BREAKER</title>
-<style>
-  @import url('\''https://fonts.googleapis.com/css2?family=Press+Start+2P&display=swap'\'');
-
-  :root{
-    --bg-deep:#0a0518;
-    --bg-panel:#140a2e;
-    --cyan:#3df5ff;
-    --magenta:#ff2e9a;
-    --yellow:#ffe15a;
-    --purple:#9b5cff;
-    --green:#5cff9b;
-    --text:#e8e3ff;
-  }
-
-  *{ box-sizing:border-box; }
-
-  html,body{
-    margin:0; padding:0; height:100%;
-    background:
-      radial-gradient(ellipse at center, #1a0f38 0%, var(--bg-deep) 70%);
-    display:flex; align-items:center; justify-content:center;
-    font-family:'\''Press Start 2P'\'', monospace;
-    color:var(--text);
-    overflow:hidden;
-  }
-
-  .cabinet{
-    position:relative;
-    background:linear-gradient(160deg,#1c1140,#0d0620);
-    border-radius:22px;
-    padding:22px 22px 28px;
-    box-shadow:
-      0 0 0 2px #3a2a6b,
-      0 0 40px rgba(155,92,255,0.35),
-      inset 0 0 30px rgba(0,0,0,0.6);
-  }
-
-  .marquee{
-    text-align:center;
-    font-size:22px;
-    letter-spacing:2px;
-    margin-bottom:14px;
-    color:var(--cyan);
-    text-shadow:
-      0 0 6px var(--cyan),
-      0 0 18px rgba(61,245,255,0.6);
-    animation:flicker 3.2s infinite;
-  }
-
-  @keyframes flicker{
-    0%,19%,21%,23%,80%,100%{ opacity:1; }
-    20%,22%{ opacity:0.55; }
-  }
-
-  .hud{
-    display:flex; justify-content:space-between;
-    font-size:11px; margin-bottom:10px; padding:0 4px;
-    color:var(--yellow);
-    text-shadow:0 0 8px rgba(255,225,90,0.6);
-  }
-
-  .screen-wrap{
-    position:relative;
-    border-radius:10px;
-    overflow:hidden;
-    box-shadow:
-      inset 0 0 0 3px #000,
-      inset 0 0 40px rgba(0,0,0,0.8);
-  }
-
-  canvas{
-    display:block;
-    background:#050311;
-  }
-
-  .scanlines{
-    pointer-events:none;
-    position:absolute; inset:0;
-    background:repeating-linear-gradient(
-      to bottom,
-      rgba(255,255,255,0.05) 0px,
-      rgba(255,255,255,0.05) 1px,
-      transparent 2px,
-      transparent 3px
-    );
-    mix-blend-mode:overlay;
-  }
-
-  .vignette{
-    pointer-events:none;
-    position:absolute; inset:0;
-    box-shadow: inset 0 0 90px 20px rgba(0,0,0,0.65);
-  }
-
-  .overlay{
-    position:absolute; inset:0;
-    display:flex; align-items:center; justify-content:center;
-    flex-direction:column;
-    gap:14px;
-    background:rgba(5,3,17,0.86);
-    text-align:center;
-    padding:20px;
-  }
-
-  .overlay.hidden{ display:none; }
-
-  .overlay h2{
-    font-size:18px; margin:0;
-    color:var(--magenta);
-    text-shadow:0 0 10px var(--magenta), 0 0 24px rgba(255,46,154,0.6);
-  }
-
-  .overlay p{
-    font-size:10px; line-height:1.9; margin:0;
-    color:var(--text);
-    max-width:280px;
-  }
-
-  .btn{
-    font-family:'\''Press Start 2P'\'', monospace;
-    font-size:11px;
-    padding:12px 18px;
-    background:var(--purple);
-    color:#0a0518;
-    border:none;
-    border-radius:6px;
-    cursor:pointer;
-    box-shadow:0 0 0 2px #0a0518, 0 0 18px rgba(155,92,255,0.7);
-    transition:transform 0.1s ease;
-  }
-  .btn:active{ transform:scale(0.95); }
-  .btn:hover{ background:var(--cyan); }
-
-  .footnote{
-    text-align:center;
-    font-size:9px;
-    margin-top:12px;
-    color:#7a6fa8;
-    letter-spacing:1px;
-  }
-
-  @media (max-width: 480px){
-    .marquee{ font-size:15px; }
-    .hud{ font-size:9px; }
-  }
-</style>
+  <meta charset="UTF-8" />
+  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
+  <title>For You, With Love</title>
+  <link rel="preconnect" href="https://fonts.googleapis.com" />
+  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
+  <link href="https://fonts.googleapis.com/css2?family=DM+Sans:wght@400;500;700&family=Playfair+Display:ital,wght@0,500;0,600;1,500;1,600&display=swap" rel="stylesheet" />
+  <style>
+    :root { --ink:#4e3e39; --muted:#8d7770; --rose:#d98282; --paper:#fffaf5; --cream:#f7eee5; --line:#eadbd0; --wine:#a95559; }
+    * { box-sizing:border-box; }
+    html { scroll-behavior:smooth; }
+    body { margin:0; color:var(--ink); background:var(--paper); font-family:"DM Sans",sans-serif; }
+    .hero { min-height:100vh; overflow:hidden; position:relative; display:grid; place-items:center; padding:40px 22px 70px; background:radial-gradient(circle at 12% 10%, #f9d9d1 0 8%, transparent 26%), radial-gradient(circle at 92% 75%, #f6dfcf 0 7%, transparent 28%), var(--cream); }
+    .petal { position:absolute; width:28px; height:18px; background:#e9aaa8; border-radius:100% 0 100% 0; opacity:.7; filter:drop-shadow(0 5px 4px #bf8b8560); animation:fall linear infinite; }
+    .petal:nth-child(1){left:8%;top:-10px;animation-duration:10s}.petal:nth-child(2){left:28%;top:15%;transform:rotate(80deg);animation-duration:13s}.petal:nth-child(3){left:85%;top:-5px;animation-duration:9s}.petal:nth-child(4){left:73%;top:28%;transform:rotate(170deg);animation-duration:12s}.petal:nth-child(5){left:45%;top:-4px;animation-duration:14s}
+    @keyframes fall { to { transform:translate(70px,110vh) rotate(320deg); } }
+    .hero-card { position:relative; z-index:1; max-width:760px; text-align:center; }
+    .eyebrow { letter-spacing:.18em; text-transform:uppercase; color:var(--wine); font-size:.72rem; font-weight:700; }
+    h1,h2 { font-family:"Playfair Display",serif; font-weight:500; margin:0; }
+    h1 { font-size:clamp(3.5rem,10vw,7.5rem); line-height:.94; letter-spacing:-.06em; }
+    h1 em { color:var(--rose); }
+    .hero p { max-width:490px; margin:28px auto 32px; color:var(--muted); font-size:1.04rem; line-height:1.75; }
+    .button { display:inline-flex; gap:10px; align-items:center; padding:14px 21px; border:1px solid var(--wine); border-radius:100px; color:#fff; background:var(--wine); text-decoration:none; font-size:.9rem; transition:.25s; }
+    .button:hover { transform:translateY(-3px); box-shadow:0 12px 24px #a9555940; }
+    .scroll { position:absolute; bottom:28px; color:var(--muted); font-size:.72rem; letter-spacing:.13em; text-transform:uppercase; }
+    .scroll::after { content:""; display:block; height:34px; width:1px; background:var(--rose); margin:10px auto 0; }
+    main { max-width:1060px; margin:auto; padding:100px 22px; }
+    .intro { text-align:center; max-width:610px; margin:0 auto 64px; }
+    h2 { font-size:clamp(2.35rem,5vw,4rem); letter-spacing:-.05em; line-height:1.05; }
+    .intro p, .letter p { color:var(--muted); line-height:1.8; }
+    .timeline { position:relative; display:grid; gap:28px; }
+    .timeline::before { content:""; position:absolute; left:50%; top:40px; bottom:40px; width:1px; background:var(--line); }
+    .memory { width:calc(50% - 30px); position:relative; padding:26px; border:1px solid var(--line); border-radius:3px 25px 3px 25px; background:#fffdfb; box-shadow:0 12px 25px #6f4f4110; transition:.3s; }
+    .memory:hover { transform:translateY(-6px) rotate(-.5deg); box-shadow:0 20px 34px #6f4f4120; }
+    .memory:nth-child(even) { margin-left:auto; border-radius:25px 3px 25px 3px; }
+    .memory::after { content:""; position:absolute; width:13px; height:13px; background:var(--rose); border:4px solid var(--paper); border-radius:50%; top:42px; }
+    .memory:nth-child(odd)::after { right:-38px; }.memory:nth-child(even)::after { left:-38px; }
+    .date { font-size:.72rem; color:var(--wine); text-transform:uppercase; letter-spacing:.13em; font-weight:700; }
+    .memory h3 { font:500 1.5rem "Playfair Display",serif; margin:10px 0 8px; }.memory p { color:var(--muted); line-height:1.6; font-size:.94rem; margin:0; }
+    .icon { position:absolute; right:24px; top:22px; color:#dfad9c; font-size:1.5rem; }
+    .letter { margin:115px auto 55px; max-width:710px; padding:clamp(30px,7vw,72px); background:linear-gradient(135deg,#fffdf9,#fff7ef); border:1px solid var(--line); position:relative; box-shadow:18px 18px 0 #f3e1d4; }
+    .letter::before { content:""; position:absolute; inset:11px; border:1px solid #f0dfd2; pointer-events:none; }.letter h2 { color:var(--wine); font-size:clamp(2.4rem,5vw,3.8rem); }.signature { font:italic 1.7rem "Playfair Display",serif; color:var(--wine); margin:25px 0 0; }
+    .promise { text-align:center; background:#f4e2d8; margin:0 -22px; padding:78px 22px; }.promise p { color:var(--muted); max-width:480px; line-height:1.7; margin:16px auto 24px; }.heart { color:var(--wine); font-size:1.2rem; }
+    footer { padding:28px; text-align:center; font-size:.78rem; color:var(--muted); background:#f4e2d8; }
+    @media (max-width:650px) { main{padding-top:72px}.timeline::before { left:18px; }.memory,.memory:nth-child(even) { width:calc(100% - 42px); margin-left:auto; }.memory::after,.memory:nth-child(even)::after { left:-31px; right:auto; }.letter { margin-top:80px; box-shadow:10px 10px 0 #f3e1d4; } }
+  </style>
 </head>
 <body>
-
-<div class="cabinet">
-  <div class="marquee">NEON BREAKER</div>
-  <div class="hud">
-    <span id="score">SCORE 0000</span>
-    <span id="level">STAGE 1</span>
-    <span id="lives">♥ ♥ ♥</span>
-  </div>
-
-  <div class="screen-wrap">
-    <canvas id="game" width="480" height="560"></canvas>
-    <div class="scanlines"></div>
-    <div class="vignette"></div>
-
-    <div class="overlay" id="startOverlay">
-      <h2>NEON BREAKER</h2>
-      <p>MOVE: ARROW KEYS / A-D / MOUSE / TOUCH<br>LAUNCH: SPACE OR CLICK<br><br>CLEAR ALL BRICKS. DON'\''T DROP THE BALL.</p>
-      <button class="btn" id="startBtn">INSERT COIN</button>
+  <header class="hero">
+    <i class="petal"></i><i class="petal"></i><i class="petal"></i><i class="petal"></i><i class="petal"></i>
+    <div class="hero-card">
+      <p class="eyebrow">a little note, from my heart</p>
+      <h1>I’m <em>sorry.</em></h1>
+      <p>I know a few words can’t undo a hurt. But I hope this small trip through our favourite moments reminds you how much you mean to me—and how much I want to do better.</p>
+      <a class="button" href="#memories">Take a walk with me <span>↓</span></a>
     </div>
-
-    <div class="overlay hidden" id="endOverlay">
-      <h2 id="endTitle">GAME OVER</h2>
-      <p id="endText">FINAL SCORE: 0</p>
-      <button class="btn" id="retryBtn">PLAY AGAIN</button>
-    </div>
-  </div>
-
-  <div class="footnote">◄ ► TO MOVE · SPACE TO LAUNCH</div>
-</div>
-
-<script>
-(function(){
-  const canvas = document.getElementById('\''game'\'');
-  const ctx = canvas.getContext('\''2d'\'');
-  const W = canvas.width, H = canvas.height;
-
-  const scoreEl = document.getElementById('\''score'\'');
-  const levelEl = document.getElementById('\''level'\'');
-  const livesEl = document.getElementById('\''lives'\'');
-  const startOverlay = document.getElementById('\''startOverlay'\'');
-  const endOverlay = document.getElementById('\''endOverlay'\'');
-  const endTitle = document.getElementById('\''endTitle'\'');
-  const endText = document.getElementById('\''endText'\'');
-  const startBtn = document.getElementById('\''startBtn'\'');
-  const retryBtn = document.getElementById('\''retryBtn'\'');
-
-  // ---------- Audio (tiny WebAudio synth, no assets needed) ----------
-  let actx;
-  function beep(freq, dur, type, vol){
-    try{
-      if(!actx) actx = new (window.AudioContext || window.webkitAudioContext)();
-      const o = actx.createOscillator();
-      const g = actx.createGain();
-      o.type = type || '\''square'\'';
-      o.frequency.value = freq;
-      g.gain.value = vol !== undefined ? vol : 0.06;
-      o.connect(g); g.connect(actx.destination);
-      o.start();
-      g.gain.exponentialRampToValueAtTime(0.0001, actx.currentTime + dur);
-      o.stop(actx.currentTime + dur);
-    }catch(e){}
-  }
-  const sfx = {
-    paddle: ()=>beep(220,0.08,'\''square'\'',0.05),
-    wall: ()=>beep(330,0.05,'\''square'\'',0.04),
-    brick: (pitch)=>beep(440 + pitch*40,0.09,'\''square'\'',0.06),
-    life: ()=>beep(140,0.3,'\''sawtooth'\'',0.08),
-    win: ()=>{ [523,659,784,1047].forEach((f,i)=>setTimeout(()=>beep(f,0.18,'\''square'\'',0.07),i*120)); },
-    lose: ()=>{ [300,220,160,100].forEach((f,i)=>setTimeout(()=>beep(f,0.22,'\''sawtooth'\'',0.08),i*140)); }
-  };
-
-  // ---------- Game constants ----------
-  const PADDLE_W = 84, PADDLE_H = 12;
-  const BALL_R = 6;
-  const BRICK_ROWS = 6, BRICK_COLS = 8;
-  const BRICK_W = 50, BRICK_H = 18, BRICK_GAP = 6;
-  const BRICK_TOP = 60, BRICK_LEFT = (W - (BRICK_COLS*(BRICK_W+BRICK_GAP)-BRICK_GAP))/2;
-
-  const rowColors = ['\''#ff2e9a'\'','\''#ff7a3d'\'','\''#ffe15a'\'','\''#5cff9b'\'','\''#3df5ff'\'','\''#9b5cff'\''];
-
-  let state = '\''idle'\''; // idle, aiming, playing, over, win
-  let score = 0, lives = 3, level = 1;
-  let paddleX = W/2 - PADDLE_W/2;
-  let ball, bricks, ballSpeed;
-
-  function initBricks(lvl){
-    const arr = [];
-    for(let r=0;r<BRICK_ROWS;r++){
-      for(let c=0;c<BRICK_COLS;c++){
-        const skip = (lvl>1 && Math.random() < 0.06 * (lvl-1));
-        arr.push({
-          x: BRICK_LEFT + c*(BRICK_W+BRICK_GAP),
-          y: BRICK_TOP + r*(BRICK_H+BRICK_GAP),
-          w: BRICK_W, h: BRICK_H,
-          color: rowColors[r % rowColors.length],
-          alive: !skip,
-          hp: r < 2 ? 1 : 1
-        });
-      }
-    }
-    return arr;
-  }
-
-  function resetBall(){
-    ball = {
-      x: paddleX + PADDLE_W/2,
-      y: H - 40 - BALL_R,
-      vx: 0,
-      vy: 0,
-      stuck: true
-    };
-  }
-
-  function newGame(){
-    score = 0; lives = 3; level = 1;
-    ballSpeed = 4.6;
-    paddleX = W/2 - PADDLE_W/2;
-    bricks = initBricks(level);
-    resetBall();
-    state = '\''aiming'\'';
-    updateHUD();
-  }
-
-  function nextLevel(){
-    level++;
-    ballSpeed += 0.6;
-    bricks = initBricks(level);
-    paddleX = W/2 - PADDLE_W/2;
-    resetBall();
-    state = '\''aiming'\'';
-    updateHUD();
-  }
-
-  function updateHUD(){
-    scoreEl.textContent = '\''SCORE '\'' + String(score).padStart(4,'\''0'\'');
-    levelEl.textContent = '\''STAGE '\'' + level;
-    livesEl.textContent = '\''♥ '\''.repeat(lives).trim();
-  }
-
-  // ---------- Input ----------
-  let leftDown=false, rightDown=false;
-  document.addEventListener('\''keydown'\'', e=>{
-    if(e.code==='\''ArrowLeft'\''||e.code==='\''KeyA'\'') leftDown=true;
-    if(e.code==='\''ArrowRight'\''||e.code==='\''KeyD'\'') rightDown=true;
-    if(e.code==='\''Space'\''){ e.preventDefault(); launch(); }
-  });
-  document.addEventListener('\''keyup'\'', e=>{
-    if(e.code==='\''ArrowLeft'\''||e.code==='\''KeyA'\'') leftDown=false;
-    if(e.code==='\''ArrowRight'\''||e.code==='\''KeyD'\'') rightDown=false;
-  });
-
-  function pointerMove(clientX){
-    const rect = canvas.getBoundingClientRect();
-    const scale = W / rect.width;
-    let x = (clientX - rect.left) * scale - PADDLE_W/2;
-    x = Math.max(0, Math.min(W-PADDLE_W, x));
-    paddleX = x;
-  }
-  canvas.addEventListener('\''mousemove'\'', e=> pointerMove(e.clientX));
-  canvas.addEventListener('\''touchmove'\'', e=>{ e.preventDefault(); pointerMove(e.touches[0].clientX); }, {passive:false});
-  canvas.addEventListener('\''mousedown'\'', launch);
-  canvas.addEventListener('\''touchstart'\'', launch);
-
-  function launch(){
-    if(state==='\''aiming'\'' && ball.stuck){
-      const angle = (-Math.PI/2) + (Math.random()*0.5 - 0.25);
-      ball.vx = Math.cos(angle) * ballSpeed;
-      ball.vy = Math.sin(angle) * ballSpeed;
-      ball.stuck = false;
-      state = '\''playing'\'';
-    }
-  }
-
-  // ---------- Update ----------
-  function update(){
-    if(leftDown) paddleX -= 7;
-    if(rightDown) paddleX += 7;
-    paddleX = Math.max(0, Math.min(W-PADDLE_W, paddleX));
-
-    if(ball.stuck){
-      ball.x = paddleX + PADDLE_W/2;
-      ball.y = H - 40 - BALL_R;
-      return;
-    }
-    if(state!=='\''playing'\'') return;
-
-    ball.x += ball.vx;
-    ball.y += ball.vy;
-
-    // walls
-    if(ball.x - BALL_R < 0){ ball.x = BALL_R; ball.vx *= -1; sfx.wall(); }
-    if(ball.x + BALL_R > W){ ball.x = W - BALL_R; ball.vx *= -1; sfx.wall(); }
-    if(ball.y - BALL_R < 0){ ball.y = BALL_R; ball.vy *= -1; sfx.wall(); }
-
-    // paddle
-    const py = H - 30;
-    if(ball.vy > 0 && ball.y + BALL_R >= py && ball.y + BALL_R <= py + PADDLE_H + 6 &&
-       ball.x >= paddleX && ball.x <= paddleX + PADDLE_W){
-      const hit = (ball.x - (paddleX + PADDLE_W/2)) / (PADDLE_W/2);
-      const angle = hit * (Math.PI/3);
-      const speed = Math.hypot(ball.vx, ball.vy);
-      ball.vx = Math.sin(angle) * speed;
-      ball.vy = -Math.abs(Math.cos(angle) * speed);
-      ball.y = py - BALL_R;
-      sfx.paddle();
-    }
-
-    // bricks
-    let aliveCount = 0;
-    for(const b of bricks){
-      if(!b.alive) continue;
-      aliveCount++;
-      if(ball.x + BALL_R > b.x && ball.x - BALL_R < b.x + b.w &&
-         ball.y + BALL_R > b.y && ball.y - BALL_R < b.y + b.h){
-        const overlapX = Math.min(ball.x+BALL_R - b.x, b.x+b.w - (ball.x-BALL_R));
-        const overlapY = Math.min(ball.y+BALL_R - b.y, b.y+b.h - (ball.y-BALL_R));
-        if(overlapX < overlapY) ball.vx *= -1; else ball.vy *= -1;
-        b.alive = false;
-        aliveCount--;
-        score += 10;
-        sfx.brick(bricks.indexOf(b) % 6);
-        updateHUD();
-        break;
-      }
-    }
-
-    // ball lost
-    if(ball.y - BALL_R > H){
-      lives--;
-      sfx.life();
-      updateHUD();
-      if(lives <= 0){
-        endGame(false);
-      } else {
-        resetBall();
-        state = '\''aiming'\'';
-      }
-    }
-
-    if(aliveCount === 0 && state==='\''playing'\''){
-      if(level >= 5){
-        endGame(true);
-      } else {
-        setTimeout(nextLevel, 400);
-        state = '\''idle'\'';
-      }
-    }
-  }
-
-  function endGame(won){
-    state = won ? '\''win'\'' : '\''over'\'';
-    won ? sfx.win() : sfx.lose();
-    endTitle.textContent = won ? '\''YOU WIN!'\'' : '\''GAME OVER'\'';
-    endText.textContent = '\''FINAL SCORE: '\'' + score;
-    endOverlay.classList.remove('\''hidden'\'');
-  }
-
-  // ---------- Draw ----------
-  function drawGlowRect(x,y,w,h,color){
-    ctx.save();
-    ctx.shadowColor = color;
-    ctx.shadowBlur = 10;
-    ctx.fillStyle = color;
-    ctx.fillRect(x,y,w,h);
-    ctx.restore();
-  }
-
-  function draw(){
-    ctx.clearRect(0,0,W,H);
-
-    ctx.strokeStyle = '\''rgba(155,92,255,0.06)'\'';
-    ctx.lineWidth = 1;
-    for(let gx=0; gx<W; gx+=24){ ctx.beginPath(); ctx.moveTo(gx,0); ctx.lineTo(gx,H); ctx.stroke(); }
-    for(let gy=0; gy<H; gy+=24){ ctx.beginPath(); ctx.moveTo(0,gy); ctx.lineTo(W,gy); ctx.stroke(); }
-
-    for(const b of bricks){
-      if(!b.alive) continue;
-      drawGlowRect(b.x,b.y,b.w,b.h,b.color);
-    }
-
-    drawGlowRect(paddleX, H-30, PADDLE_W, PADDLE_H, '\''#3df5ff'\'');
-
-    ctx.save();
-    ctx.shadowColor = '\''#ffe15a'\'';
-    ctx.shadowBlur = 14;
-    ctx.fillStyle = '\''#ffe15a'\'';
-    ctx.beginPath();
-    ctx.arc(ball.x, ball.y, BALL_R, 0, Math.PI*2);
-    ctx.fill();
-    ctx.restore();
-  }
-
-  function loop(){
-    if(state==='\''playing'\'' || state==='\''aiming'\''){
-      update();
-      draw();
-    }
-    requestAnimationFrame(loop);
-  }
-
-  startBtn.addEventListener('\''click'\'', ()=>{
-    startOverlay.classList.add('\''hidden'\'');
-    newGame();
-  });
-  retryBtn.addEventListener('\''click'\'', ()=>{
-    endOverlay.classList.add('\''hidden'\'');
-    newGame();
-  });
-
-  bricks = initBricks(1);
-  paddleX = W/2 - PADDLE_W/2;
-  resetBall();
-  draw();
-  loop();
-})();
-</script>
-
+    <div class="scroll">our story</div>
+  </header>
+  <main>
+    <section class="intro" id="memories">
+      <p class="eyebrow">the things I never want to forget</p>
+      <h2>A trip down<br><em>our</em> memory lane</h2>
+      <p>Not because the past excuses anything—but because every moment here is a reason to choose us with more care, today and tomorrow.</p>
+    </section>
+    <section class="timeline" aria-label="Our memories">
+      <article class="memory"><span class="icon">☕</span><span class="date">Chapter one</span><h3>That first long conversation</h3><p>The kind where time disappeared and even the silences felt easy. I still smile when I think about it.</p></article>
+      <article class="memory"><span class="icon">☂</span><span class="date">Chapter two</span><h3>The rainy-day detour</h3><p>We got completely lost, laughed completely too hard, and somehow made an ordinary day feel like an adventure.</p></article>
+      <article class="memory"><span class="icon">✦</span><span class="date">Chapter three</span><h3>Our tiny celebrations</h3><p>The inside jokes, late-night snacks, and little wins that became my favourite kind of tradition.</p></article>
+      <article class="memory"><span class="icon">♡</span><span class="date">Chapter four</span><h3>The way you show up</h3><p>Your patience, your warmth, your wonderfully honest heart. I notice it all—even when I haven’t said it enough.</p></article>
+    </section>
+    <section class="letter">
+      <p class="eyebrow">the part I mean most</p>
+      <h2>I should have listened better.</h2>
+      <p>I’m sorry for the moments I made you feel unseen, unheard, or less important than you are. You deserved more softness, more patience, and more effort from me.</p>
+      <p>I can’t change what happened, but I can own it. I want to learn from it, communicate with more care, and show you through my actions that your feelings are safe with me.</p>
+      <p class="signature">With all my love, always.</p>
+    </section>
+    <section class="promise"><span class="heart">♥</span><h2>Can we make new memories?</h2><p>Not perfect ones—real ones. Ones where we keep choosing kindness, honesty, and each other.</p><a class="button" href="mailto:?subject=A%20little%20note%20for%20you">Send a little love</a></section>
+  </main>
+  <footer>Made with a hopeful heart.</footer>
 </body>
 </html>
' | git apply --3way)
