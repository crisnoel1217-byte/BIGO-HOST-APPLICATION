
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>TRD BIGO Recruitment Portal</title>

<link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700;800;900&display=swap" rel="stylesheet">

<script src="https://cdn.tailwindcss.com"></script>

<style>
body{
font-family:'Inter',sans-serif;
background:#f5f7fb;
overflow-x:hidden;
}

.glow{
box-shadow:0 20px 50px rgba(255,0,128,0.25);
}

.hero-bg{
background:
linear-gradient(135deg,#ff4da6 0%,#7b61ff 50%,#4ecbff 100%);
}

.card-blur{
backdrop-filter:blur(15px);
background:rgba(255,255,255,0.12);
border:1px solid rgba(255,255,255,0.18);
}

.gradient-text{
background:linear-gradient(90deg,#fff,#ffe27a);
-webkit-background-clip:text;
-webkit-text-fill-color:transparent;
}
</style>
</head>

<body>

<!-- HERO -->
<section class="hero-bg min-h-screen relative overflow-hidden text-white">

<div class="absolute inset-0 bg-[radial-gradient(circle_at_top_right,rgba(255,255,255,0.35),transparent_35%)]"></div>

<div class="relative max-w-7xl mx-auto px-6 py-20">

<div class="grid lg:grid-cols-2 gap-14 items-center">

<!-- LEFT -->
<div>

<div class="inline-flex items-center gap-2 px-5 py-3 rounded-full card-blur mb-6 font-bold tracking-wider text-sm uppercase">
🔥 Official BIGO Recruitment
</div>

<img
src="https://upload.wikimedia.org/wikipedia/commons/thumb/7/7e/BIGO_LIVE_logo.svg/512px-BIGO_LIVE_logo.svg.png"
class="w-32 mb-6"
>

<h1 class="text-6xl md:text-7xl font-black leading-tight mb-6">
Turn Your Talent Into
<span class="block gradient-text">Real Income</span>
</h1>

<p class="text-lg md:text-xl text-white/90 leading-relaxed mb-8 max-w-2xl">
Sing, dance, livestream, entertain, and grow your fanbase with TRD BIGO Agency.
Earn income, bonuses, gifts, and professional creator support.
</p>

<!-- TIMER -->
<div class="card-blur rounded-3xl p-6 inline-block mb-8 glow">
<p class="uppercase tracking-[4px] text-sm mb-2 text-pink-100">
Recruitment Countdown
</p>

<h2 id="countdown" class="text-6xl font-black text-yellow-300">
05:00
</h2>
</div>

<!-- CTA -->
<div class="flex flex-wrap gap-4 mb-10">

<a href="#apply"
class="px-8 py-5 bg-white text-black rounded-2xl font-black hover:scale-105 transition-all duration-300">
Apply Now
</a>

<a href="#admin"
class="px-8 py-5 rounded-2xl border border-white/30 card-blur font-bold hover:bg-white/10 transition-all duration-300">
Admin Dashboard
</a>

</div>

<!-- STREAMER IMAGES -->
<div class="grid md:grid-cols-2 gap-5">

<div class="bg-white/10 rounded-3xl overflow-hidden shadow-2xl hover:scale-105 transition-all duration-300">

<img
src="https://images.unsplash.com/photo-1494790108377-be9c29b29330?q=80&w=1200&auto=format&fit=crop"
class="w-full h-64 object-cover"
>

<div class="p-5">
<h3 class="text-2xl font-black mb-2">
🎤 Singing Streamer
</h3>

<p class="text-white/80 leading-relaxed">
Showcase your voice live and receive gifts from supporters worldwide.
</p>
</div>

</div>

<div class="bg-white/10 rounded-3xl overflow-hidden shadow-2xl hover:scale-105 transition-all duration-300">

<img
src="https://images.unsplash.com/photo-1500648767791-00dcc994a43e?q=80&w=1200&auto=format&fit=crop"
class="w-full h-64 object-cover"
>

<div class="p-5">
<h3 class="text-2xl font-black mb-2">
💃 Dance Creator
</h3>

<p class="text-white/80 leading-relaxed">
Go viral with dance livestreams and interactive performances.
</p>
</div>

</div>

</div>

</div>

<!-- RIGHT -->
<div>

<div class="card-blur rounded-[35px] p-8 glow">

<div class="flex items-center justify-between mb-8">
<div>
<p class="text-white/70 mb-2">Monthly Potential</p>
<h2 class="text-6xl font-black">₱50K+</h2>
</div>

<div class="w-20 h-20 rounded-3xl bg-pink-500 flex items-center justify-center text-4xl">
🎤
</div>
</div>

<div class="grid grid-cols-2 gap-4 mb-6">

<div class="bg-black/20 rounded-3xl p-6">
<h3 class="text-3xl font-black mb-2">24/7</h3>
<p class="text-white/70">Agency Support</p>
</div>

<div class="bg-black/20 rounded-3xl p-6">
<h3 class="text-3xl font-black mb-2">1000+</h3>
<p class="text-white/70">Active Hosts</p>
</div>

</div>

<div class="bg-gradient-to-r from-pink-500 to-purple-600 rounded-3xl p-6">
<h3 class="text-2xl font-black mb-2">
No Experience Required
</h3>

<p class="text-pink-100">
We provide mentoring, coaching, and growth strategies for new streamers.
</p>
</div>

</div>

</div>

</div>
</div>

</section>

<!-- APPLICATION -->
<section id="apply" class="max-w-5xl mx-auto px-6 py-24">

<div class="text-center mb-14">
<h2 class="text-5xl font-black mb-4">
Application Form
</h2>

<p class="text-gray-500 text-lg">
Fill out the form below to apply as a BIGO Host.
</p>
</div>

<form id="applicationForm"
class="bg-white rounded-[35px] shadow-2xl border border-gray-200 p-8 md:p-12 space-y-6">

<div class="grid md:grid-cols-2 gap-6">

<div>
<label class="block mb-2 font-semibold text-gray-600">
Full Name
</label>

<input type="text" id="fullName"
required
class="w-full border border-gray-300 rounded-2xl px-5 py-4 outline-none focus:border-pink-500">
</div>

<div>
<label class="block mb-2 font-semibold text-gray-600">
Age
</label>

<input type="number" id="age"
required
class="w-full border border-gray-300 rounded-2xl px-5 py-4 outline-none focus:border-pink-500">
</div>

</div>

<div class="grid md:grid-cols-2 gap-6">

<div>
<label class="block mb-2 font-semibold text-gray-600">
Facebook Profile
</label>

<input type="text" id="facebook"
required
class="w-full border border-gray-300 rounded-2xl px-5 py-4 outline-none focus:border-pink-500">
</div>

<div>
<label class="block mb-2 font-semibold text-gray-600">
Contact Number
</label>

<input type="text" id="contact"
required
class="w-full border border-gray-300 rounded-2xl px-5 py-4 outline-none focus:border-pink-500">
</div>

</div>

<div>
<label class="block mb-2 font-semibold text-gray-600">
Complete Address
</label>

<input type="text" id="address"
required
class="w-full border border-gray-300 rounded-2xl px-5 py-4 outline-none focus:border-pink-500">
</div>

<div class="grid md:grid-cols-2 gap-6">

<div>
<label class="block mb-2 font-semibold text-gray-600">
BIGO ID
</label>

<input type="text" id="bigoId"
required
class="w-full border border-gray-300 rounded-2xl px-5 py-4 outline-none focus:border-pink-500">
</div>

<div>
<label class="block mb-2 font-semibold text-gray-600">
Government ID
</label>

<select id="governmentId"
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
<option>Postal ID</option>
<option>Voter's ID</option>

</select>

</div>

</div>

<div>
<label class="block mb-2 font-semibold text-gray-600">
Email Address
</label>

<input type="email" id="email"
required
class="w-full border border-gray-300 rounded-2xl px-5 py-4 outline-none focus:border-pink-500">
</div>

<div>
<label class="block mb-2 font-semibold text-gray-600">
Why do you want to become a BIGO Host?
</label>

<textarea id="reason"
rows="5"
class="w-full border border-gray-300 rounded-2xl px-5 py-4 outline-none focus:border-pink-500"></textarea>
</div>

<button
type="submit"
class="w-full py-5 rounded-2xl bg-gradient-to-r from-pink-500 to-purple-600 text-white text-xl font-black hover:scale-[1.02] transition-all duration-300">
Submit Application
</button>

</form>

</section>

<!-- ADMIN -->
<section id="admin" class="max-w-7xl mx-auto px-6 py-24">

<div class="flex flex-wrap gap-4 items-center justify-between mb-10">

<div>
<h2 class="text-5xl font-black mb-3">
Admin Dashboard
</h2>

<p class="text-gray-500 text-lg">
Manage applicants and export recruitment data.
</p>
</div>

<div class="flex gap-4">

<button
onclick="exportToExcel()"
class="px-6 py-4 rounded-2xl bg-green-500 text-white font-black hover:scale-105 transition-all duration-300">
Export Excel
</button>

</div>

</div>

<div class="grid md:grid-cols-4 gap-6 mb-8">

<div class="bg-white rounded-3xl p-8 shadow-xl">
<p class="text-gray-500 mb-2">Total Applicants</p>
<h3 id="totalApplicants" class="text-5xl font-black text-pink-500">
0
</h3>
</div>

<div class="bg-white rounded-3xl p-8 shadow-xl">
<p class="text-gray-500 mb-2">Agency</p>
<h3 class="text-3xl font-black">
TRD Agency
</h3>
</div>

<div class="bg-white rounded-3xl p-8 shadow-xl">
<p class="text-gray-500 mb-2">Reference BIGO ID</p>
<h3 class="text-3xl font-black text-pink-500">
TRD10_28
</h3>
</div>

<div class="bg-white rounded-3xl p-8 shadow-xl">
<p class="text-gray-500 mb-2">Recruitment Status</p>
<h3 class="text-3xl font-black text-green-500">
OPEN
</h3>
</div>

</div>

<div class="bg-white rounded-[35px] shadow-2xl overflow-hidden">

<div class="overflow-x-auto">

<table class="w-full text-left">

<thead class="bg-gray-100">
<tr>
<th class="p-5">Name</th>
<th class="p-5">Age</th>
<th class="p-5">BIGO ID</th>
<th class="p-5">Contact</th>
<th class="p-5">Government ID</th>
</tr>
</thead>

<tbody id="applicantTable">
<tr>
<td colspan="5" class="p-10 text-center text-gray-400">
No applications submitted yet.
</td>
</tr>
</tbody>

</table>

</div>

</div>

</section>

<script>

let applications = [];

const countdown = document.getElementById("countdown");

let time = 300;

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

document.getElementById("applicationForm")
.addEventListener("submit", function(e){

e.preventDefault();

const data = {
fullName: document.getElementById("fullName").value,
age: document.getElementById("age").value,
facebook: document.getElementById("facebook").value,
contact: document.getElementById("contact").value,
address: document.getElementById("address").value,
bigoId: document.getElementById("bigoId").value,
governmentId: document.getElementById("governmentId").value,
email: document.getElementById("email").value,
reason: document.getElementById("reason").value
};

applications.push(data);

document.getElementById("totalApplicants").innerText =
applications.length;

renderApplicants();

const body =
`NEW BIGO HOST APPLICATION

Full Name: ${data.fullName}
Age: ${data.age}
Facebook: ${data.facebook}
Contact Number: ${data.contact}
Address: ${data.address}
BIGO ID: ${data.bigoId}
Government ID: ${data.governmentId}
Email: ${data.email}

Reason:
${data.reason}`;

window.location.href =
`mailto:crisnoel1217@gmail.com?subject=BIGO Host Application&body=${encodeURIComponent(body)}`;

alert("Application submitted successfully!");

e.target.reset();

});

function renderApplicants(){

const table = document.getElementById("applicantTable");

if(applications.length === 0){
table.innerHTML =
`
<tr>
<td colspan="5" class="p-10 text-center text-gray-400">
No applications submitted yet.
</td>
</tr>
`;
return;
}

table.innerHTML = "";

applications.forEach((app) => {

table.innerHTML += `
<tr class="border-b border-gray-200 hover:bg-gray-50">
<td class="p-5 font-semibold">${app.fullName}</td>
<td class="p-5">${app.age}</td>
<td class="p-5 text-pink-500 font-bold">${app.bigoId}</td>
<td class="p-5">${app.contact}</td>
<td class="p-5">${app.governmentId}</td>
</tr>
`;

});

}

function exportToExcel(){

if(applications.length === 0){
alert("No applications available.");
return;
}

const headers = [
"Full Name",
"Age",
"Facebook",
"Contact",
"Address",
"BIGO ID",
"Government ID",
"Email"
];

const rows = applications.map((app) => [
app.fullName,
app.age,
app.facebook,
app.contact,
app.address,
app.bigoId,
app.governmentId,
app.email
]);

const csvContent =
[headers, ...rows]
.map(e => e.join(","))
.join("\n");

const blob = new Blob(
[csvContent],
{type:"text/csv;charset=utf-8;"}
);

const link = document.createElement("a");

const url = URL.createObjectURL(blob);

link.href = url;
link.download = "TRD_BIGO_Applicants.csv";

document.body.appendChild(link);

link.click();

document.body.removeChild(link);

}

</script>

</body>
</html>
