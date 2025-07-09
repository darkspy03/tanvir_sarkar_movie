<!DOCTYPE html>
<html lang="bn">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>🎁 Birthday Gift</title>
  <style>
    body {
      background: #011;
      color: white;
      text-align: center;
      font-family: sans-serif;
    }
    .gift {
      width: 150px;
      height: 150px;
      margin: 80px auto;
      background: url('https://cdn-icons-png.flaticon.com/512/3534/3534033.png') no-repeat center/contain;
      animation: bounce 1s infinite alternate;
      cursor: pointer;
    }
    @keyframes bounce {
      0% { transform: translateY(0); }
      100% { transform: translateY(-20px); }
    }
    .msg {
      display: none;
      margin: 20px auto;
      padding: 15px;
      width: 90%;
      max-width: 360px;
      background: rgba(255,255,255,0.1);
      border-radius: 10px;
    }
    .btn {
      display: none;
      margin: 10px;
      padding: 10px 20px;
      background: #0f0;
      border: none;
      color: black;
      font-weight: bold;
      border-radius: 8px;
    }
  </style>
</head>
<body>
  <h1>🎉 শুভ জন্মদিন! 🎂</h1>
  <div class="gift" onclick="openBox()"></div>
  <div class="msg" id="msgBox">🎁 গিফট বক্স খুলে দেখো!</div>
  <button class="btn" id="nextBtn" onclick="showNext()">পরবর্তী বার্তা দেখাও</button>

  <audio autoplay loop>
    <source src="https://www.soundhelix.com/examples/mp3/SoundHelix-Song-1.mp3" type="audio/mpeg">
  </audio>

  <script>
    const msgs = [
      "🕌 আল্লাহ তোমার জীবনকে বরকতপূর্ণ করুন 💖",
      "📿 'রব্বি যিদনী ইল্‌মা' – হে আল্লাহ, আমায় জ্ঞান বাড়িয়ে দাও",
      "🤲 প্রতিটি দিন হোক ইবাদতে ভরপুর",
      "🌙 'ইন্নাল্লাহা মা’আস্ সাবিরীন' – আল্লাহ ধৈর্যশীলদের সাথে আছেন",
      "❤️ হাদিস: 'তুমি যা ভালোবাসো, তাই হবে তোমার কিয়ামতের সাথী'",
      "✨ আল্লাহ যেন তোমাকে দুনিয়া ও আখিরাতে সফল করেন। আমিন।"
    ];
    let i = 0;
    function openBox() {
      document.querySelector('.gift').style.display = 'none';
      document.getElementById('msgBox').style.display = 'block';
      document.getElementById('nextBtn').style.display = 'inline-block';
      document.getElementById('msgBox').innerText = msgs[i];
    }
    function showNext() {
      i = (i + 1) % msgs.length;
      document.getElementById('msgBox').innerText = msgs[i];
    }
  </script>
</body>
</html>
