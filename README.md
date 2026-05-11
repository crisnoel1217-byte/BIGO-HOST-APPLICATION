
<html lang="en">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0"/>
<title>TRD BIGO Host Recruitment</title>

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

.hero{
  min-height:100vh;
  background:linear-gradient(135deg,#ff008c,#7b2ff7,#000);
  display:flex;
  align-items:center;
  justify-content:center;
  padding:40px 20px;
}

.container{
  width:100%;
  max-width:1200px;
}

.hero-grid{
  display:grid;
  grid-template-columns:1fr 1fr;
  gap:50px;
  align-items:center;
}

.badge{
  display:inline-block;
  padding:10px 18px;
  border-radius:999px;
  background:rgba(255,255,255,0.1);
  border:1px solid rgba(255,255,255,0.2);
  margin-bottom:25px;
  font-size:13px;
  font-weight:700;
  letter-spacing:1px;
}

.hero h1{
  font-size:70px;
  line-height:1;
  margin-bottom:20px;
  font-weight:900;
}

.hero h1 span{
  color:#ffc3ec;
}

.hero p{
  font-size:18px;
  color:#eee;
  line-height:1.7;
  margin-bottom:35px;
}

.btns{
  display:flex;
  gap:15px;
  flex-wrap:wrap;
}

.btn{
  padding:16px 30px;
  border-radius:18px;
  border:none;
  font-weight:800;
  cursor:pointer;
  transition:0.3s;
  text-decoration:none;
}

.btn-primary{
  background:white;
  color:black;
}

.btn-primary:hover{
  transform:translateY(-3px);
}

.btn-outline{
  background:transparent;
  border:1px solid rgba(255,255,255,0.3);
  color:white;
}

.card{
  background:rgba(255,255,255,0.08);
  border:1px solid rgba(255,255,255,0.15);
  border-radius:30px;
  padding:35px;
  backdrop-filter:blur(10px);
}

.card h2{
  font-size:50px;
  margin-top:10px;
}

.info-grid{
  display:grid;
  grid-template-columns:1fr 1fr;
  gap:15px;
  margin-top:20px;
}

.info-box{
  background:rgba(0,0,0,0.3);
  padding:20px;
  border-radius:20px;
}

.section{
  padding:100px 20px;
}

.section-title{
  text-align:center;
  margin-bottom:60px;
}

.section-title h2{
  font-size:50px;
  margin-bottom:15px;
}

.section-title p{
  color:#aaa;
  font-size:18px;
}

.benefits{
  display:grid;
  grid-template-columns:repeat(auto-fit,minmax(250px,1fr));
  gap:25px;
}

.benefit-card{
  background:#111;
  border:1px solid #222;
  border-radius:30px;
  padding:35px;
  transition:0.3s;
}

.benefit-card:hover{
  transform:translateY(-8px);
  border-color:#ff008c;
}

.benefit-card h3{
  margin:20px 0 10px;
  font-size:26px;
}

.requirements{
  display:grid;
  grid-template-columns:1fr 1fr;
  gap:50px;
  align-items:center;
}

.requirement-list{
  display:flex;
  flex-direction:column;
  gap:18px;
}

.requirement{
  background:#111;
  border:1px solid #222;
  border-radius:20px;
  padding:18px;
  display:flex;
  align-items:center;
  gap:15px;
}

.check{
  width:40px;
  height:40px;
  background:#ff008c;
  border-radius:50%;
  display:flex;
  align-items:center;
  justify-content:center;
  font-weight:bold;
}

.contact-card{
  background:linear-gradient(135deg,#ff008c,#7b2ff7);
  border-radius:30px;
  padding:40px;
}

.contact-id{
  margin-top:25px;
  background:rgba(255,255,255,0.1);
  padding:20px;
  border-radius:20px;
}

.form-container{
  max-width:850px;
  margin:auto;
  background:#111;
  border:1px solid #222;
  border-radius:35px;
  padding:40px;
}

.form-grid{
  display:grid;
  grid-template-columns:1fr 1fr;
  gap:20px;
}

.input-group{
  margin-bottom:20px;
}

label{
  display:block;
  margin-bottom:10px;
  color:#aaa;
  font-size:14px;
}

input,select,textarea{
  width:100%;
  background:black;
  border:1px solid #333;
  border-radius:18px;
  padding:16px;
  color:white;
  font-size:15px;
  outline:none;
}

input:focus,
textarea:focus,
select:focus{
  border-color:#ff008c;
}

textarea{
  resize:none;
}

.submit-btn{
  width:100%;
  padding:18px;
  border:none;
  border-radius:20px;
  background:linear-gradient(90deg,#ff008c,#7b2ff7);
  color:white;
  font-size:18px;
  font-weight:800;
  cursor:pointer;
  transition:0.3s;
}

.submit-btn:hover{
  transform:scale(1.02);
}

footer{
  padding:50px 20px;
  text-align:center;
  border-top:1px solid #222;
}

footer p{
  color:#777;
  margin-top:10px;
}

@media(max-width:900px){

.hero-grid,
.requirements,
.form-grid{
  grid-template-columns:1fr;
}

.hero h1{
  font-size:50px;
}

.section-title h2{
  font-size:38px;
}

}
</style>
</head>

<body>

<section class="hero">
<div class="container">
<div class="hero-grid">

<div>
<div class="badge">
JOIN OUR AGENCY TODAY
</div>

<h1>
Become a <span>BIGO Host</span>
</h1>

<p>
Start your streaming journey with a professional agency.
Earn income, gain followers, receive training, and grow
your online career with full support.
</p>

<div class="btns">
<a href="#apply" class="btn btn-primary">Apply Now</a>
<a href="#benefits" class="btn btn-outline">Learn More</a>
</div>
</div>

<div class="card">
<p>Monthly Potential</p>
<h2>₱50K+</h2>

<div class="info-grid">
<div class="info-box">
<h3>24/7</h3>
<p>Agency Support</p>
</div>

<div class="info-box">
<h3>1000+</h3>
<p>Active Hosts</p>
</div>
</div>

</div>

</div>
</div>
</section>

<section class="section" id="benefits">

<div class="container">

<div class="section-title">
<h2>Why Join Our Agency?</h2>
<p>
We help aspiring creators become successful BIGO streamers.
</p>
</div>

<div class="benefits">

<div class="benefit-card">
<h3>💰 High Income</h3>
<p>Earn through streaming and agency bonuses.</p>
</div>

<div class="benefit-card">
<h3>🚀 Mentorship</h3>
<p>Get guidance to grow faster on BIGO.</p>
</div>

<div class="benefit-card">
<h3>⏰ Flexible</h3>
<p>Work anytime and stream anywhere.</p>
</div>

<div class="benefit-card">
<h3>🌟 Community</h3>
<p>Friendly and supportive agency environment.</p>
</div>

</div>
</div>
</section>

<section class="section">

<div class="container requirements">

<div>

<h2 style="font-size:50px;margin-bottom:30px;">
Basic Requirements
</h2>

<div class="requirement-list">

<div class="requirement">
<div class="check">✓</div>
18 years old and above
</div>

<div class="requirement">
<div class="check">✓</div>
Stable internet connection
</div>

<div class="requirement">
<div class="check">✓</div>
Must have valid BIGO ID
</div>

<div class="requirement">
<div class="check">✓</div>
Government-issued ID required
</div>

<div class="requirement">
<div class="check">✓</div>
Friendly and confident personality
</div>

</div>

</div>

<div class="contact-card">

<h2>Ready to Start?</h2>

<p style="margin-top:15px;line-height:1.7;">
Apply now and our recruitment team will contact you.
</p>

<div class="contact-id">
<p>FOR INQUIRIES PLEASE CONTACT BIGO ID</p>
<h1 style="margin-top:10px;">TRD10_28</h1>
</div>

</div>

</div>
</section>

<section class="section" id="apply">

<div class="section-title">
<h2>Application Form</h2>
<p>Fill out the form below to apply as a BIGO Host.</p>
</div>

<div class="form-container">

<form id="applicationForm">

<div class="form-grid">

<div class="input-group">
<label>Full Name</label>
<input type="text" name="fullname" required>
</div>

<div class="input-group">
<label>Age</label>
<input type="number" name="age" required>
</div>

</div>

<div class="form-grid">

<div class="input-group">
<label>Facebook Profile</label>
<input type="text" name="facebook" required>
</div>

<div class="input-group">
<label>Contact Number</label>
<input type="text" name="contact" required>
</div>

</div>

<div class="input-group">
<label>Complete Address</label>
<input type="text" name="address" required>
</div>

<div class="form-grid">

<div class="input-group">
<label>BIGO ID</label>
<input type="text" name="bigoid" required>
</div>

<div class="input-group">
<label>Government ID</label>

<select name="governmentid" required>
<option value="">Select Government ID</option>
<option>Passport</option>
<option>National ID</option>
<option>Driver's License</option>
<option>SSS ID</option>
<option>PhilHealth ID</option>
<option>TIN ID</option>
<option>UMID</option>
<option>Postal ID</option>
<option>Voter's ID</option>
</select>

</div>

</div>

<div class="input-group">
<label>Email Address</label>
<input type="email" name="email" required>
</div>

<div class="input-group">
<label>Why do you want to become a BIGO Host?</label>
<textarea rows="5" name="reason"></textarea>
</div>

<button type="submit" class="submit-btn">
Submit Application
</button>

</form>

</div>
</section>

<footer>
<h2>TRD BIGO Agency</h2>
<p>Empowering streamers and creators worldwide.</p>
</footer>

<script>
document.getElementById("applicationForm")
.addEventListener("submit", function(e){

e.preventDefault();

const form = e.target;

const body =
`NEW BIGO HOST APPLICATION

Full Name: ${form.fullname.value}
Age: ${form.age.value}
Facebook: ${form.facebook.value}
Contact Number: ${form.contact.value}
Address: ${form.address.value}
BIGO ID: ${form.bigoid.value}
Government ID: ${form.governmentid.value}
Email: ${form.email.value}

Reason:
${form.reason.value}
`;

window.location.href =
`mailto:crisnoel1217@gmail.com?subject=BIGO Host Application&body=${encodeURIComponent(body)}`;

alert("Application prepared successfully!");

form.reset();

});
</script>

</body>
</html>
