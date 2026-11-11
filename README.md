

<!DOCTYPE html>

<html lang="ar" dir="rtl">

<head>

<meta charset="UTF-8">

<meta name="viewport" content="width=device-width, initial-scale=1">

<title>X CITY CONTROL PANEL</title>

<style>

*{box-sizing:border-box}

body{margin:0;background:#0b1020;color:#fff;font-family:Arial,sans-serif}

header{padding:24px;background:#151e32;border-bottom:1px solid #29344c}

h1{margin:0;color:#62a5ff;font-size:25px}

header p{color:#aab5c8;margin-bottom:0}

main{padding:18px;max-width:850px;margin:auto}

h2{font-size:21px}

.cards{display:grid;grid-template-columns:repeat(2,1fr);gap:12px}

.card{background:#18243a;border:1px solid #2c3c59;padding:18px;border-radius:14px}

.card p{color:#aab5c8;margin-bottom:0}

nav{display:grid;grid-template-columns:repeat(2,1fr);gap:10px;margin:20px 0}

button{background:#203552;color:white;border:1px solid #38547b;padding:14px;border-radius:10px;font-size:15px;cursor:pointer}

button:active{background:#315b91}

section{background:#151e32;padding:18px;border-radius:14px;margin-top:15px}

input{width:100%;padding:13px;background:#0b1020;color:white;border:1px solid #38547b;border-radius:9px;margin:10px 0}

.small{color:#aab5c8;font-size:13px}

</style>

</head>

<body>

<header>

<h1>X CITY</h1>

<p>CONTROL PANEL | لوحة التحكم</p>

</header>

<main>

<h2>مرحباً بك في لوحة الإدارة</h2>

<p class="small">إدارة بوت الديسكورد الخاص بك</p>

<div class="cards">

<div class="card">

<strong>حالة البوت</strong>

<p>بانتظار الربط</p>

</div>

<div class="card">

<strong>الأعضاء</strong>

<p>بانتظار الربط</p>

</div>

<div class="card">

<strong>الأوامر</strong>

<p>بانتظار الربط</p>

</div>

<div class="card">

<strong>الحماية</strong>

<p>بانتظار الربط</p>

</div>

</div>

<h2>أقسام التحكم</h2>

<nav>

<button onclick="show('welcome')">👋 الترحيب</button>

<button onclick="show('security')">🛡️ الحماية</button>

<button onclick="show('tickets')">🎫 التذاكر</button>

<button onclick="show('members')">👥 الأعضاء</button>

<button onclick="show('commands')">⚙️ الأوامر</button>

<button onclick="show('logs')">📋 السجلات</button>

</nav>

<section id="content">

<h2>الرئيسية</h2>

<p class="small">اختر أحد الأقسام للبدء.</p>

</section>

</main>

<script>

const sections={

welcome:["الترحيب","إعدادات رسائل الترحيب ستضاف هنا."],

security:["الحماية","إعدادات مكافحة السبام والحماية ستضاف هنا."],

tickets:["التذاكر","إعدادات نظام التذاكر ستضاف هنا."],

members:["الأعضاء","إدارة الأعضاء ستضاف هنا."],

commands:["الأوامر","إعدادات أوامر البوت ستضاف هنا."],

logs:["السجلات","سجل عمليات البوت سيظهر هنا."]

};

function show(id){

document.getElementById("content").innerHTML=

"<h2>"+sections[id][0]+"</h2><p class='small'>"+

sections[id][1]+"</p>";

}

</script>

</body>

</html>
