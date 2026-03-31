<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>ISU Fans Hub FINAL MAX ULTRA</title>
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<style>
body { margin:0; font-family:'Segoe UI'; background:linear-gradient(135deg,#e0f7fa,#fce4ec); }
header { background:#0a3d62; color:white; padding:20px; text-align:center; }
nav { display:flex; flex-wrap:wrap; justify-content:center; background:#1e3799; }
nav a { color:white; padding:12px; cursor:pointer; }

.section { display:none; padding:20px; }
.active { display:block; }

.game-box { background:white; padding:20px; border-radius:12px; text-align:center; }

button { padding:8px 12px; margin:6px; border:none; border-radius:8px; cursor:pointer; }

/* ANIMATIONS */
@keyframes correctPop {
0% { transform: scale(1); }
50% { transform: scale(1.2); }
100% { transform: scale(1); }
}

@keyframes wrongShake {
0% { transform: translateX(0); }
25% { transform: translateX(-6px); }
50% { transform: translateX(6px); }
75% { transform: translateX(-6px); }
100% { transform: translateX(0); }
}

.correct-anim {
background:#2ed573 !important;
color:white;
animation: correctPop 0.4s ease;
box-shadow:0 0 15px #2ed573;
}

.wrong-anim {
background:#ff4757 !important;
color:white;
animation: wrongShake 0.4s ease;
box-shadow:0 0 15px #ff4757;
}

/* COMBO */
.combo {
position:fixed;
top:25%;
left:50%;
transform:translateX(-50%);
font-size:42px;
color:#ff6b81;
animation: popFade 0.7s ease;
pointer-events:none;
}

@keyframes popFade{
0%{opacity:0; transform:translate(-50%,20px) scale(0.5);}
50%{opacity:1; transform:translate(-50%,0) scale(1.3);}
100%{opacity:0; transform:translate(-50%,-20px) scale(1);}
}
</style>
</head>

<body>

<header><h1>⛸️ ISU Fans Hub FINAL MAX ULTRA</h1></header>

<nav>
<a onclick="show('easy')">Easy</a>
<a onclick="show('hard')">Hard</a>
<a onclick="show('country')">Country</a>
<a onclick="show('timer')">Timer</a>
<a onclick="show('wordle')">Wordle</a>
<a onclick="show('leader')">Leaderboard</a>
</nav>

<div id="easy" class="section active">
<div class="game-box">
<h2>Easy</h2>
<p id="eScore"></p>
<h3 id="eQ"></h3>
<div id="eChoices"></div>
</div>
</div>

<div id="hard" class="section">
<div class="game-box">
<h2>Hard (+2)</h2>
<p id="hScore"></p>
<input id="hInput">
<button onclick="checkHard()">Guess</button>
</div>
</div>

<div id="country" class="section">
<div class="game-box">
<h2>Country</h2>
<p id="cScore"></p>
<h3 id="cQ"></h3>
<div id="cChoices"></div>
</div>
</div>

<div id="timer" class="section">
<div class="game-box">
<h2>Timer</h2>
<p id="tScore"></p>
<p id="tTime"></p>
<h3 id="tQ"></h3>
<div id="tChoices"></div>
<button onclick="startTimer()">Start</button>
</div>
</div>

<div id="wordle" class="section">
<div class="game-box">
<h2>Wordle Mode</h2>
<p id="wHint"></p>
<p id="wAttempts"></p>
<input id="wInput">
<button onclick="checkWordle()">Guess</button>
<div id="wHistory"></div>
</div>
</div>

<div id="leader" class="section">
<h2>Leaderboard</h2>
<div id="leaderList"></div>
</div>

<script>

/* NAV */
function show(id){
document.querySelectorAll('.section').forEach(s=>s.classList.remove('active'));
document.getElementById(id).classList.add('active');
}

/* SOUND */
const sCorrect=new Audio("https://actions.google.com/sounds/v1/cartoon/clang.ogg");
const sWrong=new Audio("https://actions.google.com/sounds/v1/cartoon/boing.ogg");
const sCombo=new Audio("https://actions.google.com/sounds/v1/cartoon/concussive_hit_guitar_boing.ogg");

function play(s){s.currentTime=0;s.play();}

function showCombo(text){
let d=document.createElement("div");
d.className="combo";
d.innerText=text;
document.body.appendChild(d);
setTimeout(()=>d.remove(),700);
}

/* DATA */
const skaters=[["Ilia Malinin",333.81,"USA","S"],["Yuma Kagiyama",306.67,"Japan","S"],["Shun Sato",292.08,"Japan","S"],["Mikhail Shaidorov",291.58,"Kazakhstan","S"],["Daniel Grassl",288.72,"Italy","S"],["Stephen Gogolev",281.04,"Canada","S"],["Adam Siao Him Fa",280.95,"France","S"],["Junhwan Cha",273.92,"Korea","S"],["Kao Miura",273.73,"Japan","S"],["Nika Egadze",273.00,"Georgia","S"],["Petr Gumennik",271.21,"AIN","S"],["Aleksandr Selevko",270.42,"Estonia","S"],["Sota Yamamoto",270.07,"Japan","S"],["Kevin Aymoz",269.13,"France","S"],["Kazuki Tomono",268.60,"Japan","S"],["Rio Nakata",268.47,"Japan","J"],["Nikolaj Memola",265.37,"Italy","S"],["Andrew Torgashev",259.06,"USA","S"],["Boyang Jin",258.86,"China","S"],["Jason Brown",257.81,"USA","S"],["Matteo Rizzo",256.37,"Italy","S"],["Minkyu Seo",255.91,"Korea","J"],["Lukas Britschgi",251.90,"Switzerland","S"],["Tomoki Hiwatashi",245.71,"USA","S"],["Roman Sadovsky",243.29,"Canada","S"],["Sihyeong Lee",242.52,"Korea","S"],["Jacob Sanchez",241.74,"USA","S"],["Taiga Nishino",241.23,"Japan","J"],["Vladimir Samoilov",240.83,"Poland","S"],["Georgii Reshtenko",238.27,"Czech Republic","S"],["Kaori Sakamoto",238.28,"Japan","S"],["Mone Chiba",228.47,"Japan","S"],["Ami Nakai",227.08,"Japan","S"],["Alysa Liu",226.79,"USA","S"],["Mao Shimada",218.13,"Japan","J"],["Yuna Aoki",217.39,"Japan","S"],["Niina Petrokina",216.14,"Estonia","S"],["Rion Sumiyoshi",216.06,"Japan","S"],["Nina Pinzarrone",215.20,"Belgium","S"],["Amber Glenn",214.91,"USA","S"],["Adeliia Petrosian",214.53,"AIN","S"],["Isabeau Levito",212.71,"USA","S"],["Rinka Watanabe",210.96,"Japan","S"],["Haein Lee",210.56,"Korea","S"],["Anastasiia Gubanova",209.99,"Georgia","S"],["Jia Shin",208.45,"Korea","S"],["Sofia Samodelkina",207.46,"Kazakhstan","S"],["Hana Bath",205.39,"Australia","J"],["Lara Naki Gutmann",205.12,"Italy","S"],["Loena Hendrickx",204.96,"Belgium","S"],["Sarah Everhardt",199.91,"USA","S"],["Yujae Kim",199.86,"Korea","J"],["Bradie Tennell",199.37,"USA","S"],["Mayuko Oka",199.17,"Japan","J"],["Young You",198.82,"Korea","S"],["Yuseong Kim",198.66,"Korea","J"],["Saki Miyake",196.79,"Japan","S"],["Olivia Lisko",196.23,"Finland","S"],["Mei Okada",195.82,"Japan","J"],["Starr Andrews",195.28,"USA","S"]];

/* EASY */
let eScore=0,eAns;
function newEasy(){
eAns=skaters[Math.random()*skaters.length|0];
eQ.innerText="PB: "+eAns[1];
let opts=[eAns];
while(opts.length<4){
let r=skaters[Math.random()*skaters.length|0];
if(!opts.includes(r)) opts.push(r);
}
opts.sort(()=>Math.random()-0.5);
eChoices.innerHTML="";
opts.forEach(o=>{
let b=document.createElement("button");
b.innerText=o[0];
b.onclick=()=>{
if(o===eAns){
b.classList.add("correct-anim");
play(sCorrect); showCombo("🔥");
eScore++;
}else{
b.classList.add("wrong-anim");
play(sWrong);
saveScore(eScore); eScore=0;
}
updateEasy();
setTimeout(newEasy,500);
};
eChoices.appendChild(b);
});
}
function updateEasy(){eScoreEl.innerText="Score: "+eScore;}

/* HARD */
let hAns,hScore=0;
function newHard(){
hAns=skaters[Math.random()*skaters.length|0];
hScoreEl.innerText="PB: "+hAns[1]+" | Score: "+hScore;
}
function checkHard(){
if(hAns[0].toLowerCase().includes(hInput.value.toLowerCase())){
play(sCorrect); showCombo("💥"); hScore+=2;
}else{
play(sWrong); saveScore(hScore); hScore=0;
}
newHard();
}

/* COUNTRY */
let cScore=0,cAns;
function newCountry(){
cAns=skaters[Math.random()*skaters.length|0];
cQ.innerText=cAns[0];
let countries=[...new Set(skaters.map(s=>s[2]))];
let opts=[cAns[2]];
while(opts.length<4){
let r=countries[Math.random()*countries.length|0];
if(!opts.includes(r)) opts.push(r);
}
opts.sort(()=>Math.random()-0.5);
cChoices.innerHTML="";
opts.forEach(o=>{
let b=document.createElement("button");
b.innerText=o;
b.onclick=()=>{
if(o===cAns[2]){
b.classList.add("correct-anim");
play(sCorrect); showCombo("🌍");
cScore++;
}else{
b.classList.add("wrong-anim");
play(sWrong);
saveScore(cScore); cScore=0;
}
updateCountry();
setTimeout(newCountry,500);
};
cChoices.appendChild(b);
});
}
function updateCountry(){cScoreEl.innerText="Score: "+cScore;}

/* TIMER */
let tScore=0,tTime=30,tAns,intv;
function startTimer(){
tScore=0;tTime=30;
clearInterval(intv);
nextTimer();
intv=setInterval(()=>{
tTime--;
tTimeEl.innerText="Time: "+tTime;
if(tTime<=0){clearInterval(intv); saveScore(tScore);}
},1000);
}
function nextTimer(){
tAns=skaters[Math.random()*skaters.length|0];
tQ.innerText="PB: "+tAns[1];
let opts=[tAns];
while(opts.length<4){
let r=skaters[Math.random()*skaters.length|0];
if(!opts.includes(r)) opts.push(r);
}
opts.sort(()=>Math.random()-0.5);
tChoices.innerHTML="";
opts.forEach(o=>{
let b=document.createElement("button");
b.innerText=o[0];
b.onclick=()=>{
if(o===tAns){
play(sCorrect); showCombo("⚡");
tScore++; nextTimer();
}else{
play(sWrong); tTime-=2;
}
updateTimer();
};
tChoices.appendChild(b);
});
}
function updateTimer(){
tScoreEl.innerText="Score: "+tScore;
tTimeEl.innerText="Time: "+tTime;
}

/* WORDLE */
let wAns,attempts;
function newWordle(){
wAns=skaters[Math.random()*skaters.length|0];
attempts=0;
wHistory.innerHTML="";
updateHints();
wAttempts.innerText="Attempts: 0 / 6";
}
function updateHints(){
let hints=[];
hints.push("Country: "+wAns[2]);
hints.push("Level: "+wAns[3]);
if(attempts>=1) hints.push("PB: "+wAns[1]);
if(attempts>=2) hints.push("First Letter: "+wAns[0][0]);
if(attempts>=3) hints.push("Last Letter: "+wAns[0].slice(-1));
if(attempts>=4) hints.push("Name Length: "+wAns[0].length);
if(attempts>=5) hints.push("First Name Length: "+wAns[0].split(" ")[0].length);
wHint.innerHTML=hints.join("<br>");
}
function checkWordle(){
let g=wInput.value.trim();
if(!g)return;
attempts++;
let correct=g.toLowerCase()===wAns[0].toLowerCase();
let d=document.createElement("div");
d.innerText=(correct?"✅ ":"❌ ")+g;
wHistory.appendChild(d);
updateHints();
wAttempts.innerText="Attempts: "+attempts+" / 6";

if(correct){play(sCorrect); showCombo("🎯"); saveScore(10-attempts); newWordle();}
else if(attempts>=6){play(sWrong); alert("Answer: "+wAns[0]); newWordle();}
else play(sWrong);

wInput.value="";
}

/* LEADERBOARD */
function saveScore(s){
let lb=JSON.parse(localStorage.getItem("lb")||"[]");
lb.push(s);
lb.sort((a,b)=>b-a);
lb=lb.slice(0,10);
localStorage.setItem("lb",JSON.stringify(lb));
renderLB();
}
function renderLB(){
let lb=JSON.parse(localStorage.getItem("lb")||"[]");
leaderList.innerHTML=lb.map((x,i)=>`#${i+1} - ${x}`).join("<br>");
}

/* INIT */
const eScoreEl=document.getElementById("eScore");
const cScoreEl=document.getElementById("cScore");
const tScoreEl=document.getElementById("tScore");
const tTimeEl=document.getElementById("tTime");
const hScoreEl=document.getElementById("hScore");

newEasy();newCountry();newHard();newWordle();renderLB();

</script>

</body>
</html>
