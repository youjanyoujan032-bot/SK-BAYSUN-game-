# SK-BAYSUN-game-
SK BAYSUN game is back 
<!DOCTYPE html>
<html lang="bn">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>নামাজের সময় ও হাদিস</title>
<style>
  body {
    font-family: "Noto Sans Bengali", sans-serif;
    background: linear-gradient(to bottom, #0a0a0a, #1a1a1a);
    color: #fff;
    text-align: center;
    padding: 20px;
  }
  h1 { color: #00ff99; }
  .card {
    background: #111;
    margin: 10px auto;
    padding: 15px;
    border-radius: 15px;
    width: 90%;
    max-width: 400px;
    box-shadow: 0 0 10px #00ff99;
  }
  button {
    background: #00ff99;
    border: none;
    color: #000;
    padding: 10px 20px;
    border-radius: 10px;
    margin-top: 10px;
    cursor: pointer;
    font-weight: bold;
  }
  button:hover { background: #00cc88; }
</style>
</head>
<body>

<h1>🕌 নামাজের সময়সূচী ও হাদিস 🕋</h1>

<div class="card">
  <h3>আজকের সময়সূচী</h3>
  <p id="time">বর্তমান সময়: --:--:--</p>
  <p>ফজর: <span id="fajr"></span></p>
  <p>যোহর: <span id="zuhr"></span></p>
  <p>আসর: <span id="asr"></span></p>
  <p>মাগরিব: <span id="maghrib"></span></p>
  <p>এশা: <span id="isha"></span></p>
  <p>সূর্যোদয়: <span id="sunrise"></span></p>
  <p>সূর্যাস্ত: <span id="sunset"></span></p>
</div>

<div class="card">
  <h3>📜 আজকের হাদিস</h3>
  <p id="hadith">লোড হচ্ছে...</p>
  <button onclick="nextHadith()">পরের হাদিস দেখুন 🔁</button>
</div>

<script>
  // ---- সময়সূচী ----
  const schedule = {
    fajr: "4:45 AM",
    zuhr: "12:00 PM",
    asr: "4:15 PM",
    maghrib: "5:45 PM",
    isha: "7:30 PM",
    sunrise: "6:00 AM",
    sunset: "5:40 PM"
  };

  document.getElementById("fajr").innerText = schedule.fajr;
  document.getElementById("zuhr").innerText = schedule.zuhr;
  document.getElementById("asr").innerText = schedule.asr;
  document.getElementById("maghrib").innerText = schedule.maghrib;
  document.getElementById("isha").innerText = schedule.isha;
  document.getElementById("sunrise").innerText = schedule.sunrise;
  document.getElementById("sunset").innerText = schedule.sunset;

  // ---- সময় দেখানো ----
  function updateTime() {
    const now = new Date();
    document.getElementById("time").innerText =
      "বর্তমান সময়: " + now.toLocaleTimeString('bn-BD');
  }
  setInterval(updateTime, 1000);
  updateTime();

  // ---- ২০০টি হাদিসের তালিকা ----
  const hadiths = [
    "রাসূল (সাঃ) বলেছেন, তোমাদের মধ্যে উত্তম সেই ব্যক্তি, যার আচরণ উত্তম।",
    "নামাজ জান্নাতের চাবি।",
    "সদকা গুনাহ মুছে দেয় যেমন পানি আগুন নিভিয়ে দেয়।",
    "যে আল্লাহর জন্য নম্র হয়, আল্লাহ তাকে উন্নত করেন।",
    "আল্লাহ তোমাদের চেহারা নয়, তোমাদের অন্তর দেখেন।",
    "রাগ নিয়ন্ত্রণ করা ঈমানের অংশ।",
    "জ্ঞান অর্জন করা প্রতিটি মুসলমানের জন্য ফরজ।",
    "একজন মুসলমান অন্য মুসলমানের ভাই।",
    "হাসি তোমার ভাইয়ের প্রতি সদকা।",
    "যে দয়া করে না, তার উপর দয়া করা হয় না।",
    // ...এভাবে তুমি মোট ২০০টি যোগ করতে পারবে
  ];

  let index = 0;
  function nextHadith() {
    index = (index + 1) % hadiths.length;
    document.getElementById("hadith").innerText = hadiths[index];
  }
  document.getElementById("hadith").innerText = hadiths[0];
</script>

</body>
</html>
