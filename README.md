
<html lang="en">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0"/>
<title>TRD BIGO Recruitment</title>

<link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700;800;900&display=swap" rel="stylesheet">

<script src="https://cdn.tailwindcss.com"></script>

<style>

*{
scroll-behavior:smooth;
}

body{
font-family:'Inter',sans-serif;
background:#f7f3ff;
overflow-x:hidden;
}

/* HERO BG */

.hero-bg{
background:
radial-gradient(circle at top left,#ff5fcf33,transparent 20%),
radial-gradient(circle at bottom right,#00d9ff33,transparent 25%),
linear-gradient(135deg,#13002d 0%,#30005d 35%,#5200a3 70%,#7d00ff 100%);
}

/* GLASS */

.glass{
background:rgba(255,255,255,0.12);
backdrop-filter:blur(14px);
border:1px solid rgba(255,255,255,0.15);
}

.glow{
box-shadow:0 15px 40px rgba(255,0,170,0.3);
}

.gradient-text{
background:linear-gradient(90deg,#ff4fd8,#7cf7ff);
-webkit-background-clip:text;
-webkit-text-fill-color:transparent;
}

/* FLOAT */

.float{
animation:float 4s ease-in-out infinite;
}

@keyframes float{
0%{transform:translateY(0px);}
50%{transform:translateY(-15px);}
100%{transform:translateY(0px);}
}

</style>
</head>

<body>

<!-- HERO -->
<section class="hero-bg min-h-screen text-white relative overflow-hidden">

<div class="max-w-7xl mx-auto px-6 py-10">

<!-- NAV -->
<div class="flex items-center justify-between mb-16">

<div class="flex items-center gap-4">

<img
src="/mnt/data/BIGO LOGO.png"
class="w-20 float"
/>

<div>
<h1 class="text-3xl font-black">
BIGO LIVE
</h1>

<p class="text-sm text-pink-100">
LIVE YOUR MOMENTS
</p>
</div>

</div>

<button
onclick="document.getElementById('adminSection').scrollIntoView()"
class="px-6 py-3 rounded-2xl bg-pink-500 hover:bg-pink-600 font-bold shadow-xl">
🔒 Admin Login
</button>

</div>

<!-- HERO CONTENT -->
<div class="grid lg:grid-cols-2 gap-14 items-center">

<!-- LEFT -->
<div>

<div class="inline-block px-6 py-3 rounded-full glass mb-6 font-bold uppercase tracking-widest text-sm">
🔥 Official Recruitment
</div>

<h1 class="text-6xl md:text-7xl font-black leading-tight mb-6">
Become a
<span class="block gradient-text">
BIGO HOST
</span>
</h1>

<p class="text-xl text-white/90 leading-relaxed mb-8">
Turn your talent into real income! Sing, dance, podcast,
DJ, livestream and entertain your audience while earning
through BIGO gifts and bonuses.
</p>

<!-- COUNTDOWN -->
<div class="glass rounded-3xl p-6 inline-block mb-8 glow">

<p class="uppercase tracking-[3px] text-sm mb-2 text-pink-100">
Recruitment Ends In
</p>

<h2 id="countdown"
class="text-6xl font-black text-yellow-300">
05:00
</h2>

<p class="mt-2 text-pink-100">
Minutes : Seconds
</p>

</div>

<!-- CTA -->
<div class="flex flex-wrap gap-5 mb-10">

<a href="#apply"
class="px-10 py-5 bg-gradient-to-r from-pink-500 to-purple-600 rounded-2xl text-xl font-black hover:scale-105 transition-all duration-300 glow">
APPLY NOW →
</a>

</div>

<p class="text-pink-200 font-semibold">
LIMITED SLOTS ONLY!
</p>

</div>

<!-- RIGHT -->
<div class="relative">

<!-- SINGING -->
<div class="glass rounded-[35px] overflow-hidden glow border border-pink-400 mb-6">

<div class="bg-pink-500 text-white font-bold px-5 py-2 inline-block rounded-br-2xl">
SINGING LIVE
</div>

<img
src="https://images.unsplash.com/photo-1516280440614-37939bbacd81?q=80&w=1200&auto=format&fit=crop"
class="w-full h-[330px] object-cover"
/>

</div>

<!-- DANCING -->
<div class="glass rounded-[35px] overflow-hidden glow border border-cyan-400 ml-10">

<div class="bg-cyan-400 text-black font-bold px-5 py-2 inline-block rounded-br-2xl">
DANCING LIVE
</div>

<img
src="https://images.unsplash.com/photo-1508804185872-d7badad00f7d?q=80&w=1200&auto=format&fit=crop"
class="w-full h-[280px] object-cover"
/>

</div>

</div>

</div>

</div>

</section>

<!-- BENEFITS -->
<section class="py-24 px-6 bg-[#faf7ff]">

<div class="max-w-7xl mx-auto">

<h2 class="text-center text-5xl font-black mb-16">
WHY JOIN OUR AGENCY?
</h2>

<div class="grid md:grid-cols-5 gap-6">

<div class="bg-white rounded-3xl p-8 text-center shadow-xl">
<div class="text-5xl mb-5">💎</div>
<h3 class="font-black text-xl mb-3">HIGH INCOME</h3>
<p class="text-gray-500">
Earn through gifts and performance.
</p>
</div>

<div class="bg-white rounded-3xl p-8 text-center shadow-xl">
<div class="text-5xl mb-5">⭐</div>
<h3 class="font-black text-xl mb-3">FULL SUPPORT</h3>
<p class="text-gray-500">
Guidance every step of the way.
</p>
</div>

<div class="bg-white rounded-3xl p-8 text-center shadow-xl">
<div class="text-5xl mb-5">👑</div>
<h3 class="font-black text-xl mb-3">BONUSES</h3>
<p class="text-gray-500">
Monthly rewards and incentives.
</p>
</div>

<div class="bg-white rounded-3xl p-8 text-center shadow-xl">
<div class="text-5xl mb-5">⏰</div>
<h3 class="font-black text-xl mb-3">FLEXIBLE</h3>
<p class="text-gray-500">
Stream anytime you want.
</p>
</div>

<div class="bg-white rounded-3xl p-8 text-center shadow-xl">
<div class="text-5xl mb-5">🌟</div>
<h3 class="font-black text-xl mb-3">FANBASE</h3>
<p class="text-gray-500">
Grow your audience worldwide.
</p>
</div>

</div>

</div>

</section>

<!-- APPLICATION -->
<section id="apply" class="py-24 px-6">

<div class="max-w-5xl mx-auto bg-white rounded-[40px] shadow-2xl p-10 md:p-14">

<h2 class="text-center text-5xl font-black mb-14 gradient-text">
APPLICATION FORM
</h2>

<form id="applicationForm" class="space-y-6">

<div class="grid md:grid-cols-2 gap-6">

<div>
<label class="font-bold mb-2 block">Full Name</label>

<input type="text"
id="fullName"
required
placeholder="Enter your full name"
class="w-full border border-gray-300 rounded-2xl px-5 py-4 outline-none focus:border-pink-500">
</div>

<div>
<label class="font-bold mb-2 block">Age</label>

<input type="number"
id="age"
required
placeholder="Enter your age"
class="w-full border border-gray-300 rounded-2xl px-5 py-4 outline-none focus:border-pink-500">
</div>

</div>

<div class="grid md:grid-cols-2 gap-6">

<div>
<label class="font-bold mb-2 block">Facebook Profile</label>

<input type="text"
id="facebook"
required
placeholder="https://facebook.com/yourprofile"
class="w-full border border-gray-300 rounded-2xl px-5 py-4 outline-none focus:border-pink-500">
</div>

<div>
<label class="font-bold mb-2 block">Contact Number</label>

<input type="text"
id="contact"
required
placeholder="09XXXXXXXXX"
class="w-full border border-gray-300 rounded-2xl px-5 py-4 outline-none focus:border-pink-500">
</div>

</div>

<div>
<label class="font-bold mb-2 block">Complete Address</label>

<input type="text"
id="address"
required
placeholder="House No., Street, Barangay, City"
class="w-full border border-gray-300 rounded-2xl px-5 py-4 outline-none focus:border-pink-500">
</div>

<div class="grid md:grid-cols-2 gap-6">

<div>
<label class="font-bold mb-2 block">BIGO ID</label>

<input type="text"
id="bigoId"
required
placeholder="Enter your BIGO ID"
class="w-full border border-gray-300 rounded-2xl px-5 py-4 outline-none focus:border-pink-500">
</div>

<div>
<label class="font-bold mb-2 block">Government ID</label>

<select
id="governmentId"
required
class="w-full border border-gray-300 rounded-2xl px-5 py-4 outline-none focus:border-pink-500">

<option>Select Government ID</option>
<option>Passport</option>
<option>National ID</option>
<option>Driver's License</option>
<option>SSS ID</option>
<option>PhilHealth ID</option>
<option>TIN ID</option>
<option>UMID</option>

</select>

</div>

</div>

<!-- TALENT -->
<div>

<label class="font-bold mb-2 block">
Talent Category
</label>

<select
id="talent"
required
class="w-full border border-gray-300 rounded-2xl px-5 py-4 outline-none focus:border-pink-500">

<option>Select your talent</option>
<option>🎤 Singing</option>
<option>💃 Dancing</option>
<option>🎧 DJ</option>
<option>🎙 Podcast</option>
<option>🎮 Gaming</option>
<option>😂 Comedy</option>
<option>💄 Beauty & Makeup</option>
<option>🍳 Cooking</option>
<option>🌟 Lifestyle Content</option>

</select>

</div>

<div>
<label class="font-bold mb-2 block">
Email Address
</label>

<input type="email"
id="email"
required
placeholder="yourmail@example.com"
class="w-full border border-gray-300 rounded-2xl px-5 py-4 outline-none focus:border-pink-500">
</div>

<div>
<label class="font-bold mb-2 block">
Why do you want to become a BIGO Host?
</label>

<textarea
id="reason"
rows="5"
placeholder="Write your reason here..."
class="w-full border border-gray-300 rounded-2xl px-5 py-4 outline-none focus:border-pink-500"></textarea>
</div>

<button
type="submit"
class="w-full py-5 rounded-2xl bg-gradient-to-r from-pink-500 to-purple-600 text-white text-xl font-black hover:scale-[1.02] transition-all duration-300 glow">
SUBMIT APPLICATION 🚀
</button>

</form>

</div>

</section>

<!-- ADMIN -->
<section id="adminSection"
class="py-20 px-6 bg-[#f3efff] border-t border-purple-100">

<div class="max-w-xl mx-auto">

<div class="text-center mb-10">

<div class="text-5xl mb-4">🔒</div>

<h2 class="text-4xl font-black mb-3">
ADMIN LOGIN
</h2>

<p class="text-gray-500">
This area is restricted to admin only.
</p>

</div>

<div class="bg-white rounded-[35px] p-10 shadow-2xl">

<div class="mb-6">

<label class="font-bold mb-2 block">
Username
</label>

<input type="text"
id="adminUser"
placeholder="CRIS123"
class="w-full border border-gray-300 rounded-2xl px-5 py-4">
</div>

<div class="mb-6">

<label class="font-bold mb-2 block">
Password
</label>

<input type="password"
id="adminPass"
placeholder="TRD123"
class="w-full border border-gray-300 rounded-2xl px-5 py-4">
</div>

<button
onclick="loginAdmin()"
class="w-full py-5 rounded-2xl bg-gradient-to-r from-pink-500 to-blue-500 text-white text-xl font-black">
LOGIN →
</button>

</div>

</div>

</section>

<!-- DASHBOARD -->
<section
id="dashboard"
class="hidden py-24 px-6 bg-white">

<div class="max-w-7xl mx-auto">

<div class="flex items-center justify-between mb-10">

<div>
<h2 class="text-5xl font-black mb-2">
ADMIN DASHBOARD
</h2>

<p class="text-gray-500">
TRD BIGO Recruitment System
</p>
</div>

<button
onclick="exportToExcel()"
class="px-6 py-4 rounded-2xl bg-green-500 text-white font-black">
Export Excel
</button>

</div>

<div class="grid md:grid-cols-4 gap-6 mb-8">

<div class="bg-pink-50 rounded-3xl p-8">
<p>Total Applicants</p>
<h3 id="totalApplicants"
class="text-5xl font-black text-pink-500">
0
</h3>
</div>

<div class="bg-purple-50 rounded-3xl p-8">
<p>Agency</p>
<h3 class="text-3xl font-black">
TRD Agency
</h3>
</div>

<div class="bg-cyan-50 rounded-3xl p-8">
<p>Reference BIGO ID</p>
<h3 class="text-3xl font-black">
TRD10_28
</h3>
</div>

<div class="bg-green-50 rounded-3xl p-8">
<p>Status</p>
<h3 class="text-3xl font-black text-green-500">
OPEN
</h3>
</div>

</div>

<div class="bg-white rounded-[35px] shadow-2xl overflow-hidden">

<div class="overflow-x-auto">

<table class="w-full">

<thead class="bg-gray-100">
<tr>
<th class="p-5 text-left">Name</th>
<th class="p-5 text-left">Talent</th>
<th class="p-5 text-left">BIGO ID</th>
<th class="p-5 text-left">Contact</th>
</tr>
</thead>

<tbody id="tableBody">

<tr>
<td colspan="4"
class="p-10 text-center text-gray-400">
No applicants yet.
</td>
</tr>

</tbody>

</table>

</div>

</div>

</div>

</section>

<script>

/* COUNTDOWN */

let time = 300;

const countdown = document.getElementById("countdown");

const timer = setInterval(() => {

let minutes = Math.floor(time / 60);
let seconds = time % 60;

seconds = seconds < 10 ? "0" + seconds : seconds;

countdown.innerHTML = `${minutes}:${seconds}`;

time--;

if(time < 0){
clearInterval(timer);
countdown.innerHTML = "CLOSED";
}

},1000);

/* APPLICATION */

let applications = [];

document
.getElementById("applicationForm")
.addEventListener("submit",function(e){

e.preventDefault();

const data = {
name:fullName.value,
talent:talent.value,
bigo:bigoId.value,
contact:contact.value
};

applications.push(data);

renderApplicants();

document.getElementById("totalApplicants").innerHTML =
applications.length;

alert("Application Submitted!");

const body =
`NEW BIGO APPLICATION

Name: ${fullName.value}
Age: ${age.value}
Facebook: ${facebook.value}
Contact: ${contact.value}
Address: ${address.value}
BIGO ID: ${bigoId.value}
Government ID: ${governmentId.value}
Talent: ${talent.value}
Email: ${email.value}

Reason:
${reason.value}`;

window.location.href =
`mailto:crisnoel1217@gmail.com?subject=BIGO Host Application&body=${encodeURIComponent(body)}`;

this.reset();

});

/* RENDER */

function renderApplicants(){

const table = document.getElementById("tableBody");

table.innerHTML = "";

applications.forEach((app)=>{

table.innerHTML += `
<tr class="border-b">
<td class="p-5">${app.name}</td>
<td class="p-5">${app.talent}</td>
<td class="p-5">${app.bigo}</td>
<td class="p-5">${app.contact}</td>
</tr>
`;

});

}

/* ADMIN LOGIN */

function loginAdmin(){

const user =
document.getElementById("adminUser").value;

const pass =
document.getElementById("adminPass").value;

if(user === "cris123" && pass === "TRD123"){

document
.getElementById("dashboard")
.classList.remove("hidden");

document
.getElementById("dashboard")
.scrollIntoView({behavior:"smooth"});

alert("Admin Login Success");

}else{

alert("Invalid Admin Credentials");

}

}

/* EXPORT */

function exportToExcel(){

if(applications.length === 0){
alert("No applications available.");
return;
}

const headers = [
"Name",
"Talent",
"BIGO ID",
"Contact"
];

const rows =
applications.map((app)=>[
app.name,
app.talent,
app.bigo,
app.contact
]);

const csv =
[headers,...rows]
.map(e=>e.join(","))
.join("\n");

const blob =
new Blob([csv],{
type:"text/csv;charset=utf-8;"
});

const link =
document.createElement("a");

link.href =
URL.createObjectURL(blob);

link.download =
"TRD_BIGO_APPLICANTS.csv";

document.body.appendChild(link);

link.click();

document.body.removeChild(link);

}

</script>

</body>
</html>
