
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
        <h3>5K+</h3>
        <p>Active Hosts</p>
      </div>

      <div class="stat-card">
        <h3>24/7</h3>
        <p>Support Team</p>
      </div>

      <div class="stat-card">
        <h3>₱50K+</h3>
        <p>Top Earnings</p>
      </div>
    </div>
  </div>

  <div class="hero-image">
    <img src="https://images.unsplash.com/photo-1494790108377-be9c29b29330?q=80&w=1200&auto=format&fit=crop" alt="BIGO Host">
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
</
