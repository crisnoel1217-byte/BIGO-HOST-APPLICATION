
<html lang="en">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0" />
<title>TRD BIGO HOST AGENCY</title>
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
}

.logo h1{
  font-size:28px;
  font-weight:900;
  background:linear-gradient(90deg,#ff2fb9,#00e5ff);
  -webkit-background-clip:text;
  -webkit-text-fill-color:transparent;
}

.logo p{
  color:#999;
  font-size:12px;
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

.apply-btn:hover{
  transform:translateY(-3px) scale(1.03);
}

.hero{
  min-height:100vh;
  display:grid;
  grid-template-columns:1fr 1fr;
  gap:60px;
  align-items:center;
  padding:80px 8%;
}

.badge{
  display:inline-flex;
  align-items:center;
  gap:10px;
  padding:12px 18px;
  border-radius:999px;
  background:rgba(255,255,255,0.06);
  border:1px solid rgba(255,255,255,0.08);
  margin-bottom:25px;
}

.dot{
  width:10px;
  height:10px;
  background:#00ff88;
  border-radius:50%;
  animation:pulse 1s infinite;
}

@keyframes pulse{
  0%{opacity:1}
  50%{opacity:.4}
  100%{opacity:1}
}

.hero h2{
  font-size:72px;
  font-weight:900;
  line-height:1;
  margin-bottom:25px;
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
  margin-bottom:35px;
}

.hero-buttons{
  display:flex;
  gap:20px;
  flex-wrap:wrap;
}

.secondary-btn{
  text-decoration:none;
  padding:14px 28px;
  border-radius:18px;
  border:1px solid rgba(255,255,255,0.1);
  color:white;
  background:rgba(255,255,255,0.05);
}

.stats{
  margin-top:50px;
  display:grid;
  grid-template-columns:repeat(3,1fr);
  gap:20px;
}

.stat-card{
  background:rgba(255,255,255,0.05);
  border:1px solid rgba(255,255,255,0.08);
  padding:25px;
  border-radius:24px;
  backdrop-filter:blur(20px);
}

.stat-card h3{
  font-size:32px;
  margin-bottom:8px;
}

.hero-image{
  position:relative;
}

.hero-image img{
  width:100%;
  border-radius:35px;
  height:700px;
  object-fit:cover;
  border:1px solid rgba(255,255,255,0.08);
}

.features{
  padding:100px 8%;
}

.section-title{
  text-align:center;
  margin-bottom:70px;
}

.section-title h2{
  font-size:52px;
  margin-bottom:15px;
}

.section-title p{
  color:#aaa;
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
  transition:.3s;
}

.feature-card:hover{
  transform:translateY(-8px);
  background:rgba(255,255,255,0.08);
}

.feature-card .icon{
  font-size:60px;
  margin-bottom:20px;
}

.feature-card h3{
  font-size:28px;
  margin-bottom:15px;
}

.feature-card p{
  color:#aaa;
  line-height:1.7;
}

.form-section{
  padding:100px 8%;
}

.form-container{
  max-width:1100px;
  margin:auto;
  background:rgba(255,255,255,0.05);
  border:1px solid rgba(255,255,255,0.08);
  border-radius:40px;
  padding:60px;
  backdrop-filter:blur(20px);
}

.form-title{
  text-align:center;
  margin-bottom:50px;
}

.form-title h2{
  font-size:52px;
  margin-bottom:15px;
  background:linear-gradient(90deg,#ff2fb9,#00e5ff);
  -webkit-background-clip:text;
  -webkit-text-fill-color:transparent;
}

.form-title p{
  color:#aaa;
}

form{
  display:grid;
  grid-template-columns:repeat(2,1fr);
  gap:25px;
}

.input-group{
  display:flex;
  flex-direction:column;
}

.full{
  grid-column:1/-1;
}

label{
  margin-bottom:10px;
  color:#ddd;
}

input,select{
  padding:18px;
  border-radius:18px;
  border:1px solid rgba(255,255,255,0.1);
  background:rgba(0,0,0,0.4);
  color:white;
  font-size:15px;
  outline:none;
}

input:focus,select:focus{
  border-color:#ff2fb9;
}

.submit-btn{
  grid-column:1/-1;
  padding:20px;
  border:none;
  border-radius:20px;
  background:linear-gradient(90deg,#ff008c,#7b00ff);
  color:white;
  font-size:20px;
  font-weight:900;
  cursor:pointer;
  transition:.3s;
  box-shadow:0 0 40px rgba(255,0,140,0.4);
}

.submit-btn:hover{
  transform:scale(1.02);
}

footer{
  border-top:1px solid rgba(255,255,255,0.08);
  padding:40px 8%;
  display:flex;
  justify-content:space-between;
  flex-wrap:wrap;
  gap:20px;
  color:#888;
}

.socials{
  display:flex;
  gap:20px;
}

.socials a{
  color:white;
  text-decoration:none;
}

@media(max-width:900px){
  .hero,
  .feature-grid,
  form{
    grid-template-columns:1fr;
  }

  .hero h2{
    font-size:52px;
  }

  .stats{
    grid-template-columns:1fr;
  }

  .hero-image img{
    height:500px;
  }

  .form-container{
    padding:30px;
  }
}
</style>
</head>
<body>

<header>
  <div class="logo">
    <h1>TRD BIGO HOST APPLICATION</h1>
  </div>
  <a class="apply-btn" href="#apply">Apply Now</a>
</header>

<section class="hero">
  <div>
    <h2>Become the Next <span>BIGO Star Host</span></h2>
    <p>Join our growing agency family and start your streaming journey today. Earn from ₱3K above with full support, training, and a friendly community that helps you grow, gain confidence, and shine live on BIGO.</p>
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
    <div class="feature-card">🔥 Be part of a fast-growing agency family with real support</div>
    <div class="feature-card">💰 Earn rewards, bonuses, and grow your income starting ₱3K+</div>
    <div class="feature-card">🎯 Requirements: 18+ years old, valid government ID, and dedication</div>
    <div class="feature-card">🎤 Streaming Setup: ring light, microphone, sound card, clean background</div>
    <div class="feature-card">🌟 Get coaching, tips, and guidance to become a top BIGO host</div>
    <div class="feature-card">🚀 Boost your followers, visibility, and join BIGO events & battles</div>
  </div>
</section>

<section class="form-section" id="apply">

<form action="https://formsubmit.co/crisnoel1217@gmail.com"
method="POST"
enctype="multipart/form-data"
onsubmit="showThankYou()">

<input type="hidden" name="_captcha" value="false">
<input type="hidden" name="_subject" value="New BIGO Host Application">

<input type="text" BIGO ID="First Name" placeholder="BIGO ID" required>
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
  <option>SSS ID</option>
   <option>TIN ID</option>
   <option>PHILHEALTH ID</option>
</select>

<select name="Talent" required>
  <option value="">Select Talent</option>
  <option>Singing</option>
  <option>Dancing</option>
  <option>Gaming</option>
  <option>Entertainment</option>
   <option>DJ</option>
   <option>DRAG PERFORMER</option>
</select>

<input class="full" type="file" name="Selfie Photo" accept="image/*" required>

<button type="submit">SUBMIT APPLICATION</button>

</form>

</section>

<footer>
  © 2026 PH-TRD2 AGENCY | Join. Stream. Earn. Grow | TRD10_28
</footer>

<script>
function showThankYou(){
  setTimeout(()=>{
    alert("🎉 Welcome to TRD Agency Family! Your application has been received. We will contact you soon!");
  },500);
}
</script>

</body>
</html>
