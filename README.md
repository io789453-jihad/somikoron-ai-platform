

<!DOCTYPE html>
<html lang="bn">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<meta name="theme-color" content="#101827">
<title>Somikoron AI | Learn Without Limits</title>
<style>
*{box-sizing:border-box}
body{margin:0;font-family:Arial,sans-serif;background:#0b1220;color:#f8fafc}
header{padding:20px 6%;display:flex;justify-content:space-between;align-items:center;border-bottom:1px solid #263449}
.logo{font-size:23px;font-weight:800;color:#60a5fa}
.logo span{color:white}
nav a{color:#cbd5e1;text-decoration:none;margin-left:15px;font-size:13px}
.hero{text-align:center;padding:65px 20px 35px}
.tag{color:#60a5fa;font-size:13px;letter-spacing:2px}
h1{font-size:clamp(35px,8vw,58px);margin:20px 0}
h1 span{color:#60a5fa}
.hero p{color:#aab8ca;line-height:1.8}
.panel{max-width:650px;margin:25px auto;padding:25px;background:#162337;border:1px solid #30445e;border-radius:18px}
label{display:block;margin:15px 0 8px;color:#dbeafe}
select,input{width:100%;padding:14px;border:1px solid #40536c;border-radius:9px;background:#0b1728;color:white;font-size:15px}
button{border:0;padding:14px 20px;background:#2563eb;color:white;border-radius:9px;font-size:15px;font-weight:bold;cursor:pointer}
.panel button{width:100%;margin-top:20px}
.features{max-width:900px;margin:55px auto;padding:0 18px}
.features h2{text-align:center}
.cards{display:grid;grid-template-columns:repeat(2,1fr);gap:13px}
.card{background:#162337;padding:20px;border-radius:13px;border:1px solid #30445e}
.card h3{color:#60a5fa}
.card p{color:#aab8ca;font-size:14px;line-height:1.6}
.notice{display:none;margin-top:15px;padding:13px;background:#1e3a5f;border-radius:9px;color:#dbeafe;line-height:1.6}
footer{text-align:center;padding:30px;color:#8293aa;border-top:1px solid #263449;margin-top:50px;font-size:13px}
@media(max-width:500px){nav a{margin-left:7px;font-size:11px}.cards{grid-template-columns:1fr}.panel{margin:20px 14px}}
</style>
</head>
<body>
<header>
<div class="logo">SOMIKORON <span>AI</span></div>
<nav>
<a href="#home">Home</a>
<a href="#learn">Learn</a>
<a href="#about">About</a>
</nav>
</header>

<section class="hero" id="home">
<div class="tag">INDEPENDENT AI EDUCATION PLATFORM</div>
<h1>Learn Without <span>Limits.</span></h1>
<p>তোমার পড়াশোনার বিশ্বস্ত ডিজিটাল সহকারী।<br>
Class 1–10 | বাংলা ও ইংরেজি | All Subjects</p>
</section>

<section class="panel" id="learn">
<h2>শেখা শুরু করো</h2>
<label for="class">তোমার শ্রেণি নির্বাচন করো</label>
<select id="class">
<option value="">শ্রেণি নির্বাচন</option>
<option>Class 1</option><option>Class 2</option>
<option>Class 3</option><option>Class 4</option>
<option>Class 5</option><option>Class 6</option>
<option>Class 7</option><option>Class 8</option>
<option>Class 9</option><option>Class 10</option>
</select>

<label for="subject">বিষয় নির্বাচন করো</label>
<select id="subject">
<option value="">বিষয় নির্বাচন</option>
<option>বাংলা</option><option>English</option>
<option>গণিত</option><option>উচ্চতর গণিত</option>
<option>বিজ্ঞান</option><option>পদার্থবিজ্ঞান</option>
<option>রসায়ন</option><option>জীববিজ্ঞান</option>
<option>বাংলাদেশ ও বিশ্বপরিচয়</option>
<option>ICT</option><option>ধর্ম ও নৈতিক শিক্ষা</option>
</select>

<label for="question">তোমার প্রশ্ন লিখো</label>
<input id="question" placeholder="এখানে প্রশ্ন লিখো...">

<button onclick="startLearning()">AI Tutor শুরু করো</button>
<div class="notice" id="notice"></div>
</section>

<section class="features">
<h2>তোমার শেখার সঙ্গী</h2>
<div class="cards">
<div class="card"><h3>Math Solver</h3><p>গণিতের সমস্যার ধাপে ধাপে সমাধান।</p></div>
<div class="card"><h3>Science Tutor</h3><p>বিজ্ঞানের কঠিন বিষয় সহজভাবে শেখো।</p></div>
<div class="card"><h3>English Expert</h3><p>Grammar, Vocabulary ও Writing শেখো।</p></div>
<div class="card"><h3>Exam Preparation</h3><p>MCQ, সৃজনশীল প্রশ্ন ও পরীক্ষার প্রস্তুতি।</p></div>
</div>
</section>

<footer id="about">
<strong>SOMIKORON AI</strong><br>
Independent Public AI Education Platform<br>
Built for Class 1–10 Students.
</footer>

<script>
function startLearning(){
const c=document.getElementById('class').value;
const s=document.getElementById('subject').value;
const q=document.getElementById('question').value.trim();
const n=document.getElementById('notice');
n.style.display='block';
if(!c||!s||!q){
n.textContent='অনুগ্রহ করে শ্রেণি, বিষয় এবং প্রশ্ন পূরণ করো।';
return;
}
n.textContent='তোমার নির্বাচন সংরক্ষিত হয়েছে। এটি বর্তমানে একটি Homepage Demo। AI Backend এখনো সংযুক্ত হয়নি।';
}
</script>
</body>
</html>
