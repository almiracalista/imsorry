# imsorry

<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>For My Babee ♡</title>

<style>
@import url('https://fonts.googleapis.com/css2?family=Playfair+Display:ital,wght@0,500;0,600;1,500&family=Quicksand:wght@400;500;600;700&display=swap');

* { box-sizing: border-box; }

body {
  margin: 0;
  min-height: 100vh;
  font-family: 'Quicksand', sans-serif;
  color: #875766;
  background-color: #fff6f7;
  background-image:
    radial-gradient(#e8bac7 1px, transparent 1px),
    linear-gradient(135deg, #fffafa, #f8e2e9);
  background-size: 20px 20px, cover;
  overflow-x: hidden;
}

.page {
  display: none;
  min-height: 100vh;
  padding: 30px 18px;
  align-items: center;
  justify-content: center;
  text-align: center;
}

.page.active {
  display: flex;
  animation: appear .8s ease;
}

.card {
  width: min(100%, 540px);
  padding: 35px 25px;
  border: 2px solid white;
  border-radius: 30px;
  background: rgba(255,255,255,.82);
  box-shadow: 0 10px 35px #c78a9b30;
  position: relative;
}

.card:before {
  content: "୨୧ ───── ♡ ───── ୨୧";
  display: block;
  color: #d59aaa;
  margin-bottom: 22px;
}

.kicker {
  font-size: 11px;
  letter-spacing: 3px;
  text-transform: uppercase;
  color: #c17e93;
}

h1, h2 {
  font-family: 'Playfair Display', serif;
  color: #b86f85;
  font-weight: 500;
}

h1 {
  font-size: clamp(48px, 11vw, 76px);
  line-height: 1.15;
  margin: 20px 0;
}

h2 { font-size: 34px; }

.flower {
  font-size: 70px;
  animation: float 3s ease-in-out infinite;
}

.subtitle {
  font-size: 14px;
  line-height: 1.9;
  color: #906d78;
}

.btn {
  border: none;
  padding: 13px 21px;
  border-radius: 30px;
  background: #d994a8;
  color: white;
  font-family: inherit;
  font-weight: 700;
  font-size: 13px;
  cursor: pointer;
  margin: 7px 4px;
  transition: .25s;
  box-shadow: 0 5px 12px #d994a833;
}

.btn:hover {
  transform: translateY(-3px);
  background: #bf788f;
}

.btn.secondary {
  background: #f7e5eb;
  color: #a66a7d;
}

.ribbon {
  display: inline-block;
  padding: 8px 15px;
  border-radius: 20px;
  background: #f9e7ed;
  font-size: 12px;
  margin: 4px;
}

.letter {
  background: #fff9f8;
  border: 1px dashed #e4b6c3;
  border-radius: 18px;
  padding: 20px;
  text-align: left;
  font-size: 13px;
  line-height: 1.95;
}

.signature {
  font-family: 'Playfair Display', serif;
  font-style: italic;
  margin: 20px 0;
}

.tiny {
  font-size: 10px;
  color: #bd91a0;
  margin-top: 22px;
}

.heart {
  position: fixed;
  top: -30px;
  pointer-events: none;
  z-index: 5;
  animation: fall 4s linear forwards;
}

@keyframes appear {
  from { opacity: 0; transform: translateY(20px) scale(.97); }
  to { opacity: 1; transform: translateY(0) scale(1); }
}

@keyframes float {
  50% { transform: translateY(-10px) rotate(5deg); }
}

@keyframes fall {
  to { transform: translateY(110vh) rotate(300deg); opacity: 0; }
}

@media (max-width: 480px) {
  .card { padding: 28px 19px; }
  h2 { font-size: 29px; }
  .letter { padding: 15px; }
}
</style>
</head>

<body>

<!-- PAGE 1: COVER -->
<section class="page active" id="p1">
  <div class="card">
    <div class="flower">🌸</div>
    <p class="kicker">a little something for you</p>
    <h1>haiii<br>babee ♡</h1>
    <p class="subtitle">
      hiiii, my favorite person!<br>
      i made a tiny little website just for you.<br>
      come closer, there's something i wanna say 🎀
    </p>
    <button class="btn" onclick="go(2)">
      enter, my love ♡ →
    </button>
    <p class="tiny">made with love, just for you ♡</p>
  </div>
</section>

<!-- PAGE 2: CUTE INTRO -->
<section class="page" id="p2">
  <div class="card">
    <div class="flower">🧸💗</div>
    <p class="kicker">a tiny reminder</p>
    <h2>before anything else...</h2>
    <p class="subtitle">
      i hope you know how special you are to me.
      even when things get messy, i'm still so grateful
      that i got the chance to know you.
    </p>
    <span class="ribbon">you are loved ♡</span>
    <span class="ribbon">you matter 🎀</span>
    <span class="ribbon">my favorite human</span>
    <p class="subtitle">there's something in my heart i wanna tell you...</p>
    <button class="btn secondary" onclick="go(1)">← back</button>
    <button class="btn" onclick="go(3)">open my letter 💌</button>
  </div>
</section>

<!-- PAGE 3: APOLOGY LETTER -->
<section class="page" id="p3">
  <div class="card">
    <div class="flower">💌</div>
    <p class="kicker">from my heart to yours</p>
    <h2>i'm sorry, babee.</h2>

    <div class="letter">
      <p>hey babee, ♡</p>

      <p>
        i just want to say that i'm truly sorry for the
        things i've done and for the moments when i hurt you.
        i know that saying "i'm sorry" doesn't magically
        fix everything, and i don't expect it to.
        i just want you to know that i mean it.
      </p>

      <p>
        you deserve patience, honesty, and love that makes
        you feel safe. i'm sorry for the times i didn't show
        that in the way you needed. i'm still learning,
        and i want to do better, not just with my words
        but with my actions, too.
      </p>

      <p>
        i'm genuinely proud to know you. i'm proud of the
        person you are, and i'm so grateful that our paths
        crossed. having you in my life means more to me
        than i always know how to explain.
      </p>

      <p>
        i don't want us to be perfect. i just want us to keep
        understanding each other, even when things are hard.
        i'll listen, i'll learn, and i'll try to be more
        thoughtful. you don't have to forgive me right away.
      </p>

      <p>
        thank you for being you, and thank you for the
        moments we've shared. i'm sorry, and i care about
        you so much. ♡
      </p>
    </div>

    <p class="signature">with all my love, always ♡</p>

    <button class="btn secondary" onclick="go(2)">← back</button>
    <button class="btn" onclick="go(4)">one last thing... ✨</button>
  </div>
</section>

<!-- PAGE 4: ENDING -->
<section class="page" id="p4">
  <div class="card">
    <div class="flower">🌷</div>
    <p class="kicker">a little promise</p>
    <h2>thank you for being you.</h2>

    <p class="subtitle">
      i can't promise i'll never make mistakes,
      but i can promise to keep trying to understand you,
      communicate better, and treat your heart with care.
    </p>

    <p style="font-family:'Playfair Display',serif;font-style:italic;font-size:21px;color:#b86f85">
      "i'm so glad i got to know you." ♡
    </p>

    <div class="flower">💗</div>

    <p class="subtitle">
      sending you the softest hug ever.<br>
      imagine me hugging you right now, okay? 🧸
    </p>

    <button class="btn" onclick="hug(this)">
      send a virtual hug ♡
    </button>
    <br>
    <button class="btn secondary" onclick="go(1)">
      read it again ↺
    </button>

    <p class="tiny">you'll always have a little place in my heart ♡</p>
  </div>
</section>

<script>
function go(number) {
  document.querySelectorAll('.page').forEach(page => {
    page.classList.remove('active');
  });

  document.getElementById('p' + number).classList.add('active');

  window.scrollTo({ top: 0, behavior: 'smooth' });
  sprinkle(12);
}

function sprinkle(amount = 12) {
  const symbols = ['♡', '♥', '✿', '୨୧', '🌸', '✨'];

  for (let i = 0; i < amount; i++) {
    const heart = document.createElement('span');
    heart.className = 'heart';
    heart.textContent =
      symbols[Math.floor(Math.random() * symbols.length)];

    heart.style.left = Math.random() * 100 + 'vw';
    heart.style.fontSize = (14 + Math.random() * 18) + 'px';
    heart.style.color = ['#d994a8', '#c87991', '#e8bac7'][
      Math.floor(Math.random() * 3)
    ];

    document.body.appendChild(heart);
    setTimeout(() => heart.remove(), 4200);
  }
}

function hug(button) {
  sprinkle(35);
  button.textContent = 'sending you all my love ♡';
}

setTimeout(() => sprinkle(10), 500);
</script>

</body>
</html>
