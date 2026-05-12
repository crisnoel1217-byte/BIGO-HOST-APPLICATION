
<html lang="en">
<head>
<meta charset="UTF-8" />

<title>TRD BIGO HOST AGENCY APPLICATION</title>

<link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700;800;900&display=swap" rel="stylesheet">

<style>
*{
  margin:0;
  padding:0;
  box-sizing:border-box;
  font-family:'Inter',sans-serif;
}

body{
  background:#050505;
  color:white;
  overflow-x:hidden;
}

body::before{
  content:'';
  position:fixed;
  inset:0;
  background:
  radial-gradient(circle at top left,#ff00aa33,transparent 40%),
  radial-gradient(circle at bottom right,#00e5ff22,transparent 40%),
  radial-gradient(circle at center,#7b00ff22,transparent 40%);
  z-index:-1;
  pointer-events:none;
}

header{
  display:flex;
  justify-content:space-between;
  align-items:center;
  padding:25px 8%;
  border-bottom:1px solid rgba(255,255,255,0.08);
  backdrop-filter:blur(20px);
  position:sticky;
  top:0;
  background:rgba(0,0,0,0.4);
  z-index:999;
}

html{
  scroll-behavior:smooth;
}

.logo h1{
  font-size:28px;
  font-weight:900;
  background:linear-gradient(90deg,#ff2fb9,#00e5ff);
  -webkit-background-clip:text;
  -webkit-text-fill-color:transparent;
}

.apply-btn{
  text-decoration:none;
  background:linear-gradient(90deg,#ff008c,#7b00ff);
  padding:14px 28px;
  border-radius:50px;
  color:white;
  font-weight:700;
  transition:.3s;
  box-shadow:0 0 30px rgba(255,0,140,0.4);
}

.hero{
  min-height:100vh;
  display:grid;
  grid-template-columns:1fr 1fr;
  gap:60px;
  align-items:center;
  padding:80px 8%;
}

.hero h2{
  font-size:72px;
  font-weight:900;
}

.hero h2 span{
  background:linear-gradient(90deg,#ff2fb9,#7b61ff,#00e5ff);
  -webkit-background-clip:text;
  -webkit-text-fill-color:transparent;
}

.hero p{
  color:#aaa;
  font-size:18px;
  line-height:1.7;
  margin-bottom:25px;
}

.hero img{
  width:100%;
  border-radius:35px;
  height:700px;
  object-fit:cover;
}

/* 🔴 LIVE FEED (TikTok style) */
.live-feed{
  margin-top:25px;
}

.live-title{
  font-weight:800;
  color:#ff2fb9;
  margin-bottom:10px;
  font-size:14px;
}

.feed-box{
  background:rgba(255,255,255,0.05);
  border:1px solid rgba(255,255,255,0.08);
  padding:12px;
  border-radius:20px;
  height:120px;
  overflow:hidden;
}

.feed-item{
  font-size:13px;
  color:#ddd;
  padding:5px 0;
  animation:fadeUp .5s ease;
}

@keyframes fadeUp{
  from{opacity:0; transform:translateY(10px);}
  to{opacity:1; transform:translateY(0);}
}

/* FEATURES */
.features{
  padding:100px 8%;
}

.section-title{
  text-align:center;
  margin-bottom:70px;
}

.section-title h2{
  font-size:52px;
}

.feature-grid{
  display:grid;
  grid-template-columns:repeat(3,1fr);
  gap:30px;
}

.feature-card{
  background:rgba(255,255,255,0.05);
  border:1px solid rgba(255,255,255,0.08);
  border-radius:35px;
  padding:40px;
}

/* FORM */
.form-section{
  padding:100px 8%;
}

form{
  display:grid;
  grid-template-columns:repeat(2,1fr);
  gap:25px;
  background:rgba(255,255,255,0.05);
  padding:60px;
  border-radius:40px;
  border:1px solid rgba(255,255,255,0.08);
}

input,select{
  padding:18px;
  border-radius:18px;
  border:1px solid rgba(255,255,255,0.1);
  background:rgba(0,0,0,0.4);
  color:white;
}

.full{
  grid-column:1/-1;
}

button{
  grid-column:1/-1;
  padding:20px;
  border:none;
  border-radius:20px;
  background:linear-gradient(90deg,#ff008c,#7b00ff);
  color:white;
  font-size:20px;
  font-weight:900;
  cursor:pointer;
}

/* FOOTER */
footer{
  padding:40px 8%;
  text-align:center;
  color:#888;
}

@media(max-width:900px){
  .hero, .feature-grid, form{
    grid-template-columns:1fr;
  }

  .hero h2{
    font-size:45px;
  }
}
</style>
</head>

<body>

<header>
  <div class="logo">
    <h1>TRD BIGO HOST APPLICATION SITE</h1>
  </div>
  <a class="apply-btn" href="#apply">Apply Now</a>
</header>

<section class="hero">
  <div>
    <h2>Become the Next <span>BIGO Star</span></h2>
    <p>Join our agency family and start streaming. Earn from ₱3K above with full support, training, and a friendly community.</p>

    <!-- 🔴 LIVE FEED -->
    <div class="live-feed">
      <div class="live-title">🔴 LIVE Applicants Joining</div>
      <div class="feed-box" id="feedBox"></div>
    </div>
  </div>

  <div>
    <img src="https://images.unsplash.com/photo-1524504388940-b1c1722653e1?q=80&w=1200&auto=format&fit=crop">
  </div>
</section>

<section class="features">
  <div class="section-title">
    <h2>What You Get & Requirements</h2>
  </div>

  <div class="feature-grid">
    <div class="feature-card">🔥 Agency family support</div>
    <div class="feature-card">💰 Earn ₱3K+ and grow</div>
    <div class="feature-card">🔞 Must be 18+ with valid ID</div>
    <div class="feature-card">🎤 Ring light, mic, sound card setup,Internet connection</div>
    <div class="feature-card">🌟 Coaching & guidance</div>
    <div class="feature-card">🚀 Events & BIGO exposure</div>
  </div>
</section>

<section class="form-section" id="apply">

<form action="https://formsubmit.co/crisnoel1217@gmail.com"
method="POST"
enctype="multipart/form-data"
onsubmit="showThankYou()">

<input type="hidden" name="_captcha" value="false">
<input type="hidden" name="_subject" value="New BIGO Host Application">

  <input type="text" Bigo Id="First Name" placeholder="Bigo ID" required>
<input type="text" name="First Name" placeholder="First Name" required>
<input type="text" name="Last Name" placeholder="Last Name" required>
<input type="text" name="Middle Name" placeholder="Middle Name">

<input type="number" name="Age" placeholder="Age" required>
<input type="text" name="Address" placeholder="Address" required>

<input type="tel" name="CP Number" placeholder="CP Number" required>
<input type="email" name="Email" placeholder="Email Address" required>

<select name="Government ID" required>
  <option value="">Select Government ID</option>
  <option>National ID</option>
  <option>Passport</option>
  <option>Driver License</option>
  <option>Philhealth</option>
  <option>TIN ID</option>
</select>

<select name="Talent" required>
  <option value="">Select Talent</option>
  <option>Singing</option>
  <option>Dancing</option>
  <option>Gaming</option>
  <option>Dj</option>
  <option>Funny</option>
  <option>Entertainment</option>
</select>

<input class="full" type="file" name="Selfie Photo" accept="image/*" required>

<button type="submit">SUBMIT APPLICATION</button>

</form>

</section>

<footer>
  © 2026 TRD BIGO HOST AGENCY
</footer>

<script>
function showThankYou(){
  setTimeout(()=>{
    alert("🎉 Application received! Welcome to TRD Agency Family!");
  },500);
}

/* TikTok-style live feed */
const names = [
  "Maria just applied 🎤",
  "John joined agency 🔥",
  "Alexa submitted form 💖",
  "Kevin applied now 🚀",
  "Angel joined TRD 🌟",
  "Kikay just applied 🎤",
  "Avie joined agency 🔥",
  "Regine submitted form 💖",
  "Ela applied now 🚀",
  "Xaez joined agency 🔥"
  "Mark uploaded selfie 📸"
];

function addFeed(){
  const box = document.getElementById("feedBox");

  const item = document.createElement("div");
  item.className = "feed-item";
  item.innerText = names[Math.floor(Math.random()*names.length)];

  box.prepend(item);

  if(box.children.length > 5){
    box.removeChild(box.lastChild);
  }
}

setInterval(addFeed, 2000);
</script>

</body>
</html>
