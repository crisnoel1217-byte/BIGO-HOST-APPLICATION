<!DOCTYPE html>
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
    <h1>TRD BIGO HOST</h1>
    <p>Modern Recruitment Platform</p>
  </div>

  <a href="#apply" class="apply-btn">Apply Now</a>
</header>

<section class="hero">
  <div>
    <div class="badge">
      <div class="dot"></div>
      <span>Now Hiring BIGO Live Hosts</span>
    </div>

    <h2>
      Become a <br>
      <span>BIGO Star</span>
    </h2>

    <p>
      Join our next-generation streaming agency and grow your audience, income, and online presence with full support and professional coaching.
    </p>

    <div class="hero-buttons">
      <a href="#apply" class="apply-btn">Apply as Host</a>
      <a href="#features" class="secondary-btn">Learn More</a>
    </div>

    <div class="stats">
      <div class="stat-card">
        <h3>ACTIVE</h3>
        <p>Agency & Family</p>
      </div>

      <div class="stat-card">
        <h3>24/7</h3>
        <p>Support Team</p>
      </div>

      <div class="stat-card">
        <h3>₱3K\+</h3>
        <p>Earnings Start From</p>
      </div>
    </div>
  </div>

  <div class="hero-image">
    <img src="https://images.unsplash.com/photo-1524504388940-b1c1722653e1?q=80&w=1200&auto=format&fit=crop" alt="BIGO Streaming Host with Microphone">
  </div>
</section>

<section class="features" id="features">
  <div class="section-title">
    <h2>Why Become a BIGO Host?</h2>
    <p>Experience exciting opportunities, income potential, and online fame.</p>
  </div>

  <div class="feature-grid">
    <div class="feature-card">
      <div class="icon">🎁</div>
      <h3>Monthly Bonuses</h3>
      <p>Earn exciting bonuses, gifts, diamonds, and incentives every month based on your streaming performance.</p>
    </div>

    <div class="feature-card">
      <div class="icon">🌍</div>
      <h3>Worldwide Audience</h3>
      <p>Connect with viewers globally and grow your fanbase through entertaining livestream content.</p>
    </div>

    <div class="feature-card">
      <div class="icon">🔥</div>
      <h3>Trending Events</h3>
      <p>Join BIGO competitions, PK battles, live challenges, and featured events to boost visibility.</p>
    </div>
  </div>
</section>

<section class="features">
  <div class="section-title">
    <h2>Host Requirements</h2>
    <p>Before applying, make sure you meet the following requirements.</p>
  </div>

  <div class="feature-grid">
    <div class="feature-card">
      <div class="icon">🪪</div>
      <h3>Valid Government ID</h3>
      <p>Applicants must provide a valid government-issued ID such as National ID, Passport, Driver’s License, Postal ID, or PhilHealth ID.</p>
    </div>

    <div class="feature-card">
      <div class="icon">🔞</div>
      <h3>18 Years Old Above</h3>
      <p>All applicants must be 18 years old or above to qualify as an official BIGO Host.</p>
    </div>

    <div class="feature-card">
      <div class="icon">📱</div>
      <h3>Good Internet & Phone</h3>
      <p>You need a stable internet connection and a smartphone or device capable of livestreaming smoothly.</p>
    </div>
  </div>
</section>

<section class="features">
  <div class="section-title">
    <h2>Recommended Livestream Setup</h2>
    <p>Professional setup helps attract more viewers and supporters.</p>
  </div>

  <div class="feature-grid">
    <div class="feature-card">
      <div class="icon">💡</div>
      <h3>Ring Light</h3>
      <p>Use a ring light or soft lighting setup for a brighter and more professional appearance during livestreams.</p>
    </div>

    <div class="feature-card">
      <div class="icon">🎵</div>
      <h3>Sound Card & Music</h3>
      <p>Improve your livestream quality with a sound card, microphone, and background music setup for better entertainment.</p>
    </div>

    <div class="feature-card">
      <div class="icon">✨</div>
      <h3>Neat Background</h3>
      <p>Maintain a clean and aesthetic streaming background to create a professional and attractive livestream environment.</p>
    </div>
  </div>
</section>

<section class="features" id="features">
  <div class="section-title">
    <h2>Why Join Our Agency?</h2>
    <p>Everything you need to become a successful BIGO streamer.</p>
  </div>

  <div class="feature-grid">
    <div class="feature-card">
      <div class="icon">🎤</div>
      <h3>Daily Coaching</h3>
      <p>Get professional training and streaming strategies from experienced managers.</p>
    </div>

    <div class="feature-card">
      <div class="icon">💰</div>
      <h3>High Earnings</h3>
      <p>Receive salary bonuses, gifts, commissions, and event rewards.</p>
    </div>

    <div class="feature-card">
      <div class="icon">🚀</div>
      <h3>Fast Growth</h3>
      <p>Boost your followers and become a recognized creator on BIGO Live.</p>
    </div>
  </div>
</section>

<section class="form-section" id="apply">
  <div class="form-container">
    <div class="form-title">
      <h2>BIGO Host Application Form</h2>
      <p>Fill out the form below and submit your application.</p>
    </div>

    <form
      action="https://formsubmit.co/crisnoel1217@gmail.com"
      method="POST"
      onsubmit="showThankYou()"
    >

      <input type="hidden" name="_captcha" value="false">
      <input type="hidden" name="_template" value="table">
      <input type="hidden" name="_subject" value="New BIGO Host Application">

      <div class="input-group">
        <label>First Name</label>
        <input type="text" name="First Name" required>
      </div>

      <div class="input-group">
        <label>Last Name</label>
        <input type="text" name="Last Name" required>
      </div>

      <div class="input-group">
        <label>Middle Name</label>
        <input type="text" name="Middle Name">
      </div>

      <div class="input-group">
        <label>Age</label>
        <input type="number" name="Age" required>
      </div>

      <div class="input-group full">
        <label>Address</label>
        <input type="text" name="Address" required>
      </div>

      <div class="input-group">
        <label>CP Number</label>
        <input type="tel" name="CP Number" required>
      </div>

      <div class="input-group">
        <label>Email Address</label>
        <input type="email" name="Email Address" required>
      </div>

      <div class="input-group">
        <label>Valid Government ID</label>
        <select name="Government ID" required>
          <option value="">Select ID</option>
          <option>Passport</option>
          <option>National ID</option>
          <option>Driver's License</option>
          <option>PhilHealth ID</option>
          <option>Postal ID</option>
          <option>TIN ID</option>
          <option>SSS ID</option>
        </select>
      </div>

      <div class="input-group">
        <label>Talent Category</label>
        <select name="Talent Category" required>
          <option value="">Select Talent</option>
          <option>Singing</option>
          <option>Dancing</option>
          <option>Gaming</option>
          <option>Entertainment</option>
          <option>Comedy</option>
          <option>Beauty Content</option>
          <option>Vlogging</option>
          <option>DJ</option>
          <option>DRAG PERFORMANCE</option>
        </select>
      </div>

      <div class="input-group full">
        <label>Upload Selfie Photo Requirement</label>
        <input type="file" name="Selfie Photo" accept="image/*" required>
        <small style="color:#999;margin-top:10px;line-height:1.6;">
          Please upload a clear selfie photo with good lighting. Avoid filters, masks, or unclear images.
        </small>
      </div>

      <button type="submit" class="submit-btn">
        SUBMIT APPLICATION
      </button>
    </form>
  </div>
</section>

<footer>
  <div>
    © 2026 PH-TRD2 AGENCY . All rights reserved.
    BIGO ID: TRD10_28
  </div>

  <div class="socials">
    <a href="#">Facebook</a>
    <a href="#">Telegram</a>
    <a href="#">Instagram</a>
  </div>
</footer>

<script>
function showThankYou(){
  setTimeout(() => {
    alert('🎉 Thank you for applying to TRD BIGO HOST AGENCY! We will review your application and contact you soon.');
  },500);
}
</script>

</body>
</html>
