
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

header{
  display:flex;
  justify-content:space-between;
  align-items:center;
  padding:20px 8%;
  position:sticky;
  top:0;
  background:rgba(0,0,0,0.6);
  backdrop-filter:blur(20px);
  z-index:1000;
  border-bottom:1px solid rgba(255,255,255,0.08);
}

.logo h1{
  font-size:26px;
  font-weight:900;
  background:linear-gradient(90deg,#ff2fb9,#00e5ff);
  -webkit-background-clip:text;
  -webkit-text-fill-color:transparent;
}

.apply-btn{
  background:linear-gradient(90deg,#ff008c,#7b00ff);
  padding:12px 22px;
  border-radius:50px;
  text-decoration:none;
  color:white;
  font-weight:700;
}

.hero{
  padding:80px 8%;
  display:grid;
  grid-template-columns:1fr 1fr;
  gap:50px;
}

.hero h2{
  font-size:60px;
  font-weight:900;
}

.hero h2 span{
  background:linear-gradient(90deg,#ff2fb9,#00e5ff);
  -webkit-background-clip:text;
  -webkit-text-fill-color:transparent;
}

.hero p{
  color:#aaa;
  margin-top:15px;
  line-height:1.6;
}

.hero img{
  width:100%;
  border-radius:30px;
}

.features{
  padding:80px 8%;
}

.section-title{
  text-align:center;
  margin-bottom:40px;
}

.section-title h2{
  font-size:40px;
}

.feature-grid{
  display:grid;
  grid-template-columns:repeat(3,1fr);
  gap:20px;
}

.feature-card{
  background:rgba(255,255,255,0.05);
  padding:25px;
  border-radius:25px;
  border:1px solid rgba(255,255,255,0.08);
}

.form-section{
  padding:80px 8%;
}

form{
  display:grid;
  grid-template-columns:repeat(2,1fr);
  gap:20px;
  background:rgba(255,255,255,0.05);
  padding:40px;
  border-radius:30px;
  border:1px solid rgba(255,255,255,0.08);
  backdrop-filter:blur(20px);
}

input,select{
  padding:15px;
  border-radius:15px;
  border:1px solid rgba(255,255,255,0.1);
  background:rgba(0,0,0,0.4);
  color:white;
}

.full{
  grid-column:1/-1;
}

button{
  grid-column:1/-1;
  padding:18px;
  border:none;
  border-radius:20px;
  background:linear-gradient(90deg,#ff008c,#7b00ff);
  color:white;
  font-weight:900;
  font-size:18px;
  cursor:pointer;
}

footer{
  padding:30px 8%;
  text-align:center;
  color:#888;
}

@media(max-width:900px){
  .hero, .feature-grid, form{
    grid-template-columns:1fr;
  }
  .hero h2{
    font-size:40px;
  }
}
</style>
</head>

<body>

<header>
  <div class="logo">
    <h1>TRD BIGO HOST</h1>
  </div>
  <a class="apply-btn" href="#apply">Apply Now</a>
</header>

<section class="hero">
  <div>
    <h2>Become a <span>BIGO Host</span></h2>
    <p>Join our agency family and start streaming. Earnings start from ₱3K above with full support.</p>
  </div>

  <div>
    <img src="https://images.unsplash.com/photo-1524504388940-b1c1722653e1?q=80&w=1200&auto=format&fit=crop">
  </div>
</section>

<section class="features">
  <div class="section-title">
    <h2>Requirements</h2>
  </div>

  <div class="feature-grid">
    <div class="feature-card">🪪 Valid Government ID</div>
    <div class="feature-card">🔞 Must be 18 years old above</div>
    <div class="feature-card">🎤 Setup: Ring light, mic, sound card</div>
    <div class="feature-card">Internet connection</div>
  </div>
</section>

<section class="form-section" id="apply">

<form action="https://formsubmit.co/crisnoel1217@gmail.com"
method="POST"
enctype="multipart/form-data"
onsubmit="showThankYou()">

<input type="hidden" name="_captcha" value="false">
<input type="hidden" name="_subject" value="New BIGO Host Application">

<input type="text" bigo ID="First Name" placeholder="Bigo ID" required>
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
  <option>Philhealth</option>
  <option>TIN ID</option>
</select>

<select name="Talent" required>
  <option value="">Select Talent</option>
  <option>Singing</option>
  <option>Dancing</option>
  <option>Gaming</option>
  <option>Entertainment</option>
  <option>DJ</option>
  <option>DRAG PERFORMANCE</option>
</select>

<input class="full" type="file" name="Selfie Photo" accept="image/*" required>

<button type="submit">SUBMIT APPLICATION</button>

</form>

</section>

<footer>
  © 2026 PH-TRD2 AGENCY BIGO ID: TRD10_28
</footer>

<script>
function showThankYou(){
  setTimeout(()=>{
    alert("🎉 Thank you for applying! We will review your application soon.");
  },500);
}
</script>

</body>
</html>
