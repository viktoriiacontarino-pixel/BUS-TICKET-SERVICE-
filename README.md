```html
<!DOCTYPE html>
<html lang="uk">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>BUS TICKET SERVICE</title>
<style>
body{margin:0;background:#111;color:white;font-family:Arial,sans-serif;line-height:1.6}
header,footer{text-align:center;background:#080808;padding:25px}
header{border-bottom:3px solid #daba68}
h1,h2,h3{color:#e5c16c}
nav{text-align:center;background:#222;padding:12px}
nav a{color:#e5c16c;margin:7px;display:inline-block}
.hero{text-align:center;padding:45px 15px;background:#332817}
section{max-width:750px;margin:auto;padding:20px}
.card{background:#222;padding:20px;margin:15px 0;border:1px solid #8c7137;border-radius:10px}
input,select,textarea{display:block;width:100%;box-sizing:border-box;padding:12px;margin:8px 0 16px;background:#111;color:white;border:1px solid #777;border-radius:5px}
label{color:#e5c16c}
button,.button{display:inline-block;background:#e5c16c;color:#111;padding:12px 18px;border:0;border-radius:6px;font-weight:bold;text-decoration:none;cursor:pointer}
form button{width:100%}
.small{font-size:13px;color:#ccc}
.whatsapp{position:fixed;bottom:15px;right:12px;background:#25d366;color:white;padding:13px;border-radius:30px;text-decoration:none}
</style>
</head>
<body>

<header>
<h1>BUS TICKET SERVICE</h1>
<p>🇺🇦 Україна — 🇮🇹 Італія — 🇪🇺 Європа</p>
</header>

<nav>
<a href="#tickets">Автобусні квитки</a>
<a href="#booking">Бронювання</a>
<a href="#cancel">Скасування</a>
<a href="#services">Послуги</a>
<a href="#contact">Контакти</a>
</nav>

<div class="hero">
<h2>Подорожуй Європою! 🚌</h2>
<p>Квитки, туризм та допомога в Італії</p>
<a class="button" href="#booking">Забронювати квиток</a>
</div>

<section id="tickets">
<h2>🚌 Автобусні рейси</h2>

<div class="card">
<h3>Дніпро 🇺🇦 — Салерно 🇮🇹</h3>
<p>Дні відправлення: вівторок і четвер.</p>
<p>Ціна та наявність місць уточнюються.</p>
<button onclick="route('Дніпро','Салерно')">Забронювати</button>
</div>

<div class="card">
<h3>Наші перевізники</h3>
<p>🚌 AL TRANS</p>
<p>🚌 Bus Trans</p>
<p>🚌 KLR</p>
<p class="small">Розклад і вартість підтверджуються перед бронюванням.</p>
</div>
</section>

<section id="booking">
<h2>🎫 Заявка на бронювання</h2>
<div class="card">
<form id="bookingForm">
<label>Ім'я та прізвище</label>
<input id="name" required>

<label>Телефон</label>
<input id="phone" type="tel" required>

<label>Звідки</label>
<input id="from" required>

<label>Куди</label>
<input id="to" required>

<label>Дата поїздки</label>
<input id="date" type="date" required>

<label>Кількість пасажирів</label>
<select id="passengers">
<option>1</option><option>2</option><option>3</option>
<option>4</option><option>5</option><option>6</option>
</select>

<label>Перевізник</label>
<select id="carrier">
<option>Будь-який</option>
<option>AL TRANS</option>
<option>Bus Trans</option>
<option>KLR</option>
</select>

<label>Коментар</label>
<textarea id="comments"></textarea>

<button type="submit">Надіслати заявку у WhatsApp</button>
<p class="small">Це заявка, а не підтверджений квиток. Онлайн-оплати немає.</p>
</form>
</div>
</section>

<section id="cancel">
<h2>❌ Скасування бронювання</h2>
<div class="card">
<form id="cancelForm">
<label>Номер бронювання</label>
<input id="bookingNumber" required>

<label>Ім'я та прізвище</label>
<input id="cancelName" required>

<label>Причина скасування</label>
<select id="reason">
<option>Змінилися плани</option>
<option>Зміна дати</option>
<option>Інша причина</option>
</select>

<button type="submit">Надіслати запит на скасування</button>
<p class="small">Дочекайтеся підтвердження скасування.</p>
</form>
</div>
</section>

<section id="services">
<h2>🇮🇹 Послуги в Італії</h2>
<div class="card">
<h3>🏠 Допомога з житлом</h3>
<p>Допомога з пошуком житла та орендою.</p>
</div>
<div class="card">
<h3>💼 Допомога з роботою</h3>
<p>Інформаційна допомога з пошуком вакансій.</p>
</div>
<div class="card">
<h3>🗺️ Туризм у Лаціо</h3>
<p>Туристичний супровід та організація поїздок.</p>
</div>
<div class="card">
<h3>🗣️ Перекладач і медіатор</h3>
<p>Мовний супровід та допомога у спілкуванні з установами.</p>
</div>
<div class="card">
<h3>🏥 Супровід до лікарні</h3>
<p>Допомога з організацією візиту та перекладом.</p>
</div>
<div class="card">
<h3>📄 Посвідка на проживання та громадянство</h3>
<p>Інформаційна допомога з документами та процедурами оформлення.</p>
</div>
</section>

<section id="contact">
<h2>📲 Контакти</h2>
<div class="card">
<p>BUS TICKET SERVICE</p>
<p>Телефон: +39 327 731 4977</p>
<a class="button" href="https://wa.me/393277314977" target="_blank">Написати у WhatsApp</a>
</div>
</section>

<footer>
<p>BUS TICKET SERVICE</p>
<p>Україна 🇺🇦 — Італія 🇮🇹 — Європа 🇪🇺</p>
</footer>

<a class="whatsapp" href="https://wa.me/393277314977" target="_blank">WhatsApp</a>

<script>
const whatsapp="393277314977";

function route(from,to){
document.getElementById('from').value=from;
document.getElementById('to').value=to;
document.getElementById('booking').scrollIntoView({behavior:'smooth'});
}

document.getElementById('date').min=new Date().toLocaleDateString('en-CA');

document.getElementById('bookingForm').addEventListener('submit',function(e){
e.preventDefault();
const g=id=>document.getElementById(id).value;
const msg="ЗАЯВКА BUS TICKET SERVICE\n"+
"Ім'я: "+g('name')+"\n"+
"Телефон: "+g('phone')+"\n"+
"Маршрут: "+g('from')+" — "+g('to')+"\n"+
"Дата: "+g('date')+"\n"+
"Пасажирів: "+g('passengers')+"\n"+
"Перевізник: "+g('carrier')+"\n"+
"Коментар: "+g('comments')+"\n"+
"Прошу перевірити наявність місць.";
window.open("https://wa.me/"+whatsapp+"?text="+encodeURIComponent(msg),"_blank");
});

document.getElementById('cancelForm').addEventListener('submit',function(e){
e.preventDefault();
const g=id=>document.getElementById(id).value;
const msg="ЗАПИТ НА СКАСУВАННЯ\n"+
"Номер бронювання: "+g('bookingNumber')+"\n"+
"Ім'я: "+g('cancelName')+"\n"+
"Причина: "+g('reason')+"\n"+
"Прошу підтвердити скасування.";
window.open("https://wa.me/"+whatsapp+"?text="+encodeURIComponent(msg),"_blank");
});
</script>
</body>
</html>
```

