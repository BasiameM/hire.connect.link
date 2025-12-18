<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>HIRELINK | South Africa Jobs</title>

<meta name="description" content="Find jobs in South Africa from top companies. Apply directly on company websites.">
<meta name="keywords" content="South Africa jobs, Sasol jobs, PepsiCo jobs, Clicks careers, Planet Fitness jobs">
<meta name="robots" content="index, follow">

<link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;500;700&display=swap" rel="stylesheet">

<style>
body{margin:0;font-family:Roboto;background:#121212;color:#fff}
header{background:#1f1f1f;padding:16px 20px;border-bottom:2px solid #00e5ff}
.logo-wrap{display:flex;align-items:center;gap:15px}
.logo svg{width:64px;height:64px}
h1{margin:0;color:#00e5ff;letter-spacing:2px;font-size:1.8em}
.tagline{font-size:0.85em;color:#7ddcff;font-style:italic}

main{max-width:1200px;margin:20px auto;padding:0 15px}
section{background:#1e1e1e;padding:20px;border-radius:12px;margin-bottom:20px}

.search-bar{display:flex;gap:10px;flex-wrap:wrap}
.search-bar input{flex:1;padding:10px;border-radius:6px;border:none}
.search-bar button{padding:10px 16px;border-radius:6px;border:none;background:#00e5ff;font-weight:600;cursor:pointer}

.company{background:#0077cc;border-radius:10px;padding:18px;margin-bottom:15px}
.company h3{margin:0 0 10px 0}

.job{display:flex;justify-content:space-between;align-items:center;border-bottom:1px solid #005fa3;padding:8px 0}
.job:last-child{border:none}

.apply{background:#00e5ff;color:#000;padding:6px 14px;border-radius:6px;text-decoration:none;font-weight:600}

footer{background:#1f1f1f;padding:20px;text-align:center;border-top:2px solid #00e5ff;font-size:0.85em}

@media(max-width:768px){
.job{flex-direction:column;align-items:flex-start;gap:8px}
.search-bar{flex-direction:column}
}
</style>
</head>

<body oncontextmenu="return false">

<header>
  <div class="logo-wrap">
    <div class="logo">
      <svg viewBox="0 0 100 100">
        <defs>
          <linearGradient id="g" x1="0" y1="0" x2="1" y2="1">
            <stop offset="0%" stop-color="#00e5ff"/>
            <stop offset="100%" stop-color="#005fa3"/>
          </linearGradient>
        </defs>
        <circle cx="50" cy="50" r="46" fill="url(#g)" stroke="#fff" stroke-width="2"/>
        <rect x="28" y="18" width="14" height="64" fill="#fff"/>
        <rect x="58" y="18" width="14" height="64" fill="#fff"/>
        <line x1="30" y1="48" x2="70" y2="52" stroke="#fff" stroke-width="4"/>
      </svg>
    </div>
    <div>
      <h1>HIRELINK</h1>
      <div class="tagline">Connecting job seekers to real opportunities in South Africa</div>
    </div>
  </div>
</header>

<main>

<section>
<h2>Search Jobs</h2>
<div class="search-bar">
<input type="text" id="search" placeholder="Search job, company or location">
<button id="searchBtn">Search</button>
</div>
</section>

<!-- Google AdSense (replace IDs when approved) -->
<section style="text-align:center">
<ins class="adsbygoogle"
     style="display:block"
     data-ad-client="ca-pub-XXXXXXXXXXXX"
     data-ad-slot="YYYYYYYYYY"
     data-ad-format="auto"
     data-full-width-responsive="true"></ins>
</section>

<section>
<h2>Top Companies Hiring Now</h2>
<div id="jobs"></div>
</section>

<footer>
<p>© 2025 HIRELINK. All Rights Reserved.</p>
</footer>

<script>
document.addEventListener("DOMContentLoaded",function(){

const jobsData=[
{company:"Sasol",jobs:[
{title:"Process Operator",location:"Sasolburg, Free State",url:"https://jobs.sasol.com/"},
{title:"Laboratory Technician",location:"Secunda, Mpumalanga",url:"https://jobs.sasol.com/"},
{title:"Electrical Engineer",location:"Sasolburg, Free State",url:"https://jobs.sasol.com/"}
]},
{company:"PepsiCo South Africa",jobs:[
{title:"Sales Representative",location:"Johannesburg, Gauteng",url:"https://www.pepsicojobs.com/southafrica/jobs/"},
{title:"Warehouse Operator",location:"Durban, KwaZulu-Natal",url:"https://www.pepsicojobs.com/southafrica/jobs/"},
{title:"Marketing Specialist",location:"Cape Town, Western Cape",url:"https://www.pepsicojobs.com/southafrica/jobs/"}
]},
{company:"Clicks Group",jobs:[
{title:"Retail Store Manager",location:"Cape Town, Western Cape",url:"https://www.clicks.co.za/careers"},
{title:"Pharmacy Assistant",location:"Johannesburg, Gauteng",url:"https://www.clicks.co.za/careers"},
{title:"IT Support Specialist",location:"Pretoria, Gauteng",url:"https://www.clicks.co.za/careers"}
]},
{company:"Planet Fitness",jobs:[
{title:"Receptionist",location:"Claremont, Western Cape",url:"https://www.planetfitness.co.za/careers/"},
{title:"Personal Trainer",location:"Durbanville, Western Cape",url:"https://www.planetfitness.co.za/careers/"},
{title:"Club Manager",location:"Johannesburg, Gauteng",url:"https://www.planetfitness.co.za/careers/"}
]},
{company:"Metropolitan",jobs:[
{title:"Financial Advisor",location:"Johannesburg, Gauteng",url:"https://www.metropolitan.co.za/careers/"},
{title:"Insurance Consultant",location:"Cape Town, Western Cape",url:"https://www.metropolitan.co.za/careers/"},
{title:"Claims Officer",location:"Durban, KwaZulu-Natal",url:"https://www.metropolitan.co.za/careers/"}
]}
];

function render(data){
const c=document.getElementById("jobs");
c.innerHTML="";
data.forEach(co=>{
let h=`<div class="company"><h3>${co.company}</h3>`;
co.jobs.forEach(j=>{
h+=`<div class="job">
<span>${j.title} – ${j.location}</span>
<a class="apply" href="${j.url}" target="_blank">APPLY</a>
</div>`;
});
h+="</div>";
c.innerHTML+=h;
});
}

render(jobsData);

document.getElementById("searchBtn").onclick=function(){
const q=document.getElementById("search").value.toLowerCase();
render(jobsData.map(c=>({
company:c.company,
jobs:c.jobs.filter(j=>(j.title+j.location+c.company).toLowerCase().includes(q))
})).filter(c=>c.jobs.length));
};

});
</script>

</body>
</html>
