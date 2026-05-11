<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>TRD BIGO CRM SYSTEM</title>

<!-- FIREBASE -->
<script src="https://www.gstatic.com/firebasejs/10.7.1/firebase-app-compat.js"></script>
<script src="https://www.gstatic.com/firebasejs/10.7.1/firebase-auth-compat.js"></script>
<script src="https://www.gstatic.com/firebasejs/10.7.1/firebase-firestore-compat.js"></script>
<script src="https://www.gstatic.com/firebasejs/10.7.1/firebase-storage-compat.js"></script>

<link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;800;900&display=swap" rel="stylesheet">

<style>
body{
margin:0;
font-family:Inter;
background:#0b0b10;
color:white;
}

/* HEADER */
.header{
position:fixed;
top:0;
width:100%;
display:flex;
justify-content:space-between;
padding:15px;
background:rgba(0,0,0,0.6);
backdrop-filter:blur(10px);
z-index:10;
}

/* FEED */
.feed{
margin-top:60px;
height:100vh;
overflow-y:scroll;
scroll-snap-type:y mandatory;
}

.card{
height:100vh;
scroll-snap-align:start;
display:flex;
flex-direction:column;
justify-content:flex-end;
padding:20px;
position:relative;
background-size:cover;
background-position:center;
}

.card::before{
content:"";
position:absolute;
inset:0;
background:linear-gradient(to top,rgba(0,0,0,0.85),transparent);
}

.content{
position:relative;
z-index:2;
}

.name{
font-size:28px;
font-weight:900;
}

.talent{
opacity:0.8;
}

/* BUTTON */
.btn{
padding:10px;
border:none;
border-radius:15px;
margin-top:5px;
cursor:pointer;
font-weight:700;
}

.approve{background:green;color:white}
.reject{background:red;color:white}

/* ADMIN */
.adminPanel{
display:none;
padding:20px;
background:#111;
}

.item{
background:#1a1a25;
padding:15px;
margin-bottom:10px;
border-radius:15px;
display:flex;
gap:10px;
align-items:center;
}

img{
width:60px;
height:60px;
border-radius:50%;
object-fit:cover;
}

</style>
</head>

<body>

<!-- HEADER -->
<div class="header">
<div>🔥 TRD CRM</div>
<div onclick="adminLogin()">Admin</div>
</div>

<!-- TIKTOK FEED -->
<div class="feed" id="feed"></div>

<!-- ADMIN DASHBOARD -->
<div class="adminPanel" id="adminPanel">

<h1>📊 CRM DASHBOARD</h1>

<div style="margin-bottom:10px">
<button onclick="filter('all')">All</button>
<button onclick="filter('pending')">Pending</button>
<button onclick="filter('approved')">Approved</button>
<button onclick="filter('rejected')">Rejected</button>
</div>

<div id="crmList"></div>

</div>

<script>

/* FIREBASE CONFIG */
const firebaseConfig = {
apiKey: "YOUR_API_KEY",
authDomain: "YOUR_PROJECT.firebaseapp.com",
projectId: "YOUR_PROJECT_ID",
storageBucket: "YOUR_PROJECT.appspot.com"
};

firebase.initializeApp(firebaseConfig);

const db = firebase.firestore();

/* LOAD DATA */
let allApps = [];

db.collection("applications").onSnapshot((snap)=>{

allApps = [];

let feed = document.getElementById("feed");
feed.innerHTML = "";

snap.forEach(doc=>{
let a = doc.data();
let id = doc.id;

allApps.push({id,...a});

/* TIKTOK FEED */
feed.innerHTML += `
<div class="card" style="background-image:url('${a.selfie}')">

<div class="content">
<div class="talent">🎭 ${a.talent}</div>
<div class="name">${a.name}</div>

<button class="btn" onclick="apply('${id}')">
Apply Now
</button>

</div>

</div>
`;

});

renderCRM(allApps);

});

/* APPLY ACTION */
function apply(id){
db.collection("applications").doc(id).update({
status:"applied"
});
}

/* ADMIN LOGIN */
function adminLogin(){

let pass = prompt("Enter Admin Password");

if(pass==="TRD123"){
document.getElementById("adminPanel").style.display="block";
alert("CRM Opened");
}else{
alert("Wrong Password");
}

}

/* CRM RENDER */
function renderCRM(data){

let box = document.getElementById("crmList");
box.innerHTML = "";

data.forEach(a=>{

box.innerHTML += `
<div class="item">

<img src="${a.selfie}">

<div style="flex:1">
<b>${a.name}</b>
<p>${a.talent}</p>
<p>${a.bigo}</p>

<span style="color:${
a.status==="approved"?"lime":
a.status==="rejected"?"red":"orange"
}">
${a.status || "pending"}
</span>

</div>

<div>
<button class="btn approve" onclick="approve('${a.id}')">✔</button>
<button class="btn reject" onclick="reject('${a.id}')">❌</button>
</div>

</div>
`;

});

}

/* APPROVE / REJECT */
function approve(id){
db.collection("applications").doc(id).update({
status:"approved"
});
}

function reject(id){
db.collection("applications").doc(id).update({
status:"rejected"
});
}

/* FILTER */
function filter(type){

if(type==="all"){
renderCRM(allApps);
return;
}

renderCRM(allApps.filter(a=>a.status===type));

}

</script>

</body>
</html>
