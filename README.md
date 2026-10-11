# Yiu-are-awesome-
Your are strong 

<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<meta name="theme-color" content="#251448">
<title>A Little Letter for Meee 💌</title>

<style>
@import url('https://fonts.googleapis.com/css2?family=Nunito:wght@400;600;700;800&family=Pacifico&display=swap');

:root {
  --pink: #ff75b7;
  --purple: #9a75ff;
  --cream: #fff8ee;
  --ink: #34264f;
}

* { box-sizing: border-box; }

body {
  margin: 0;
  min-height: 100vh;
  font-family: 'Nunito', sans-serif;
  color: var(--ink);
  background:
    radial-gradient(circle at 15% 15%, #ffd3eb 0, transparent 32%),
    radial-gradient(circle at 85% 80%, #c6b7ff 0, transparent 35%),
    linear-gradient(145deg, #fff0f8, #e9e0ff, #d7edff);
  overflow-x: hidden;
}

button { font: inherit; cursor: pointer; }

.app {
  width: min(100%, 480px);
  min-height: 100vh;
  margin: auto;
  padding: 25px 20px 35px;
  position: relative;
  overflow: hidden;
}

.screen {
  display: none;
  min-height: calc(100vh - 60px);
  flex-direction: column;
  align-items: center;
  justify-content: center;
  text-align: center;
  animation: appear .65s ease both;
}

.screen.active { display: flex; }

@keyframes appear {
  from { opacity: 0; transform: translateY(15px); }
  to { opacity: 1; transform: translateY(0); }
}

.eyebrow {
  font-size: 12px;
  font-weight: 800;
  letter-spacing: 3px;
  text-transform: uppercase;
  color: #7858b4;
}

h1, h2, p { margin-top: 0; }

h1 {
  font-size: clamp(29px, 8vw, 42px);
  line-height: 1.25;
  margin: 15px 0;
}

h2 { font-size: 26px; margin-bottom: 15px; }

.script {
  font-family: 'Pacifico', cursive;
  font-weight: 400;
  color: #e94e9e;
}

.subtitle {
  font-size: 15px;
  line-height: 1.8;
  max-width: 330px;
  color: #655677;
}

.envelope {
  position: relative;
  width: 220px;
  height: 150px;
  margin: 30px auto;
  background: linear-gradient(140deg, #ffb4d7, #c8b5ff);
  border-radius: 12px;
  box-shadow: 0 18px 40px #8e69b844;
  display: grid;
  place-items: center;
  font-size: 68px;
  animation: float 3s ease-in-out infinite;
}

.envelope:after {
  content: "♥";
  position: absolute;
  font-size: 33px;
  color: #fff;
  text-shadow: 0 2px 6px #b64b9d;
}

@keyframes float {
  0%,100% { transform: translateY(0) rotate(-2deg); }
  50% { transform: translateY(-12px) rotate(2deg); }
}

.btn {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  gap: 8px;
  border: 0;
  border-radius: 50px;
  padding: 14px 23px;
  margin: 7px 4px;
  color: white;
  font-weight: 800;
  background: linear-gradient(110deg, #ff69ae, #9b73ff);
  box-shadow: 0 8px 20px #b66dc844;
  transition: transform .2s, box-shadow .2s;
}

.btn:hover { transform: translateY(-3px); }
.btn:active { transform: scale(.97); }

.btn.secondary {
  background: #fff;
  color: #7652b0;
  border: 1px solid #e6d7ff;
  box-shadow: none;
}

.letter {
  width: 100%;
  padding: 27px 23px;
  text-align: left;
  border-radius: 22px;
  background: rgba(255, 251, 242, .96);
  border: 2px solid #fff;
  box-shadow: 0 15px 45px #6e4c9b25;
  line-height: 1.9;
  font-size: 15px;
  position: relative;
}

.letter:before {
  content: "✿  ✦  ♡";
  display: block;
  color: #f17cb9;
  text-align: right;
  letter-spacing: 7px;
  margin-bottom: 17px;
}

.letter p { margin-bottom: 14px; }

.highlight {
  background: linear-gradient(transparent 45%, #ffd5eb 45%);
  font-weight: 800;
  font-size: 17px;
}

.signature {
  text-align: right;
  color: #e454a0;
  font-family: 'Pacifico', cursive;
  font-size: 19px;
}

.card {
  width: 100%;
  padding: 22px;
  border: 1px solid #ffffff;
  border-radius: 22px;
  background: #ffffffbd;
  box-shadow: 0 12px 30px #7660a322;
  text-align: left;
  margin: 10px 0;
}

.reason {
  display: flex;
  align-items: flex-start;
  gap: 12px;
  margin: 15px 0;
  line-height: 1.6;
}

.number {
  flex-shrink: 0;
  width: 31px;
  height: 31px;
  border-radius: 50%;
  display: grid;
  place-items: center;
  background: linear-gradient(130deg, #ffacd6, #c4b4ff);
  font-weight: 800;
}

.meter {
  width: 100%;
  height: 12px;
  border-radius: 30px;
  background: #eadfff;
  overflow: hidden;
  margin: 15px 0;
}

.meter span {
  display: block;
  height: 100%;
  width: 0;
  border-radius: inherit;
  background: linear-gradient(90deg, #ff71b6, #a481ff);
  transition: width 1.3s ease;
}

.big-heart {
  font-size: 95px;
  filter: drop-shadow(0 8px 10px #d56ea844);
  animation: heartbeat 1.2s infinite;
}

@keyframes heartbeat {
  0%,100% { transform: scale(1); }
  15% { transform: scale(1.12); }
  30% { transform: scale(1); }
  45% { transform: scale(1.08); }
}

.star {
  position: fixed;
  top: -30px;
  z-index: 10;
  pointer-events: none;
  animation: fall linear forwards;
}

@keyframes fall {
  to { transform: translateY(110vh) rotate(600deg); opacity: 0; }
}

footer {
  text-align: center;
  font-size: 12px;
  color: #806e9a;
  margin-top: 18px;
}

.small { font-size: 12px; color: #88789d; }

@media (max-width: 360px) {
  .app { padding: 20px 14px; }
  .letter { padding: 22px 17px; }
  .envelope { width: 190px; height: 135px; }
}
</style>
</head>

<body>
<main class="app">

  <!-- PAGE 1: WELCOME -->
  <section class="screen active" id="home">
    <div class="eyebrow">A tiny surprise for you</div>
    <h1>A little letter for my<br>
      <span class="script">very special friend...</span>
    </h1>

    <p class="subtitle">
      Hey meee! ♡<br>
      I made a little corner of the internet
      just to remind you how special you are.
    </p>

    <div class="envelope" aria-label="A gift envelope">💌</div>

    <p class="subtitle">
      No special occasion needed.<br>
      You deserve a little happiness today.
    </p>

    <button class="btn" onclick="openLetter()">
      Open your letter 💌
    </button>
    <footer>Made with love, just for you ♡</footer>
  </section>

  <!-- PAGE 2: THE LETTER -->
  <section class="screen" id="letterPage">
    <div class="eyebrow">Please read this slowly</div>
    <h1 class="script">Hey, meee! ♡</h1>

    <article class="letter">
      <p>Dear meee,</p>

      <p>
        I just wanted to remind you of something
        that you might sometimes forget.
      </p>

      <p>
        <span class="highlight">
          Tum bhot strong ho, tum sab kar sakti ho. ♡
        </span>
      </p>

      <p>
        Even when things feel difficult, I hope
        you remember how much strength you have.
        You don't have to be perfect, and you
        don't have to figure everything out today.
      </p>

      <p>
        Take your time. Learn at your own pace.
        Celebrate your little wins, and be kind
        to yourself on the difficult days too.
      </p>

      <p>
        You deserve happiness, peace, good people
        and beautiful things in your life.
        Never forget that your dreams matter.
      </p>

      <p>
        And whenever you need a reminder,
        come back and read this again.
      </p>

      <p class="signature">
        Always cheering for you ♡
      </p>
    </article>

    <button class="btn" onclick="goTo('reasons')">
      One more little surprise ✨
    </button>
    <button class="btn secondary" onclick="goTo('home')">
      ← Back
    </button>
  </section>

  <!-- PAGE 3: REASONS -->
  <section class="screen" id="reasons">
    <div class="eyebrow">A little reminder</div>
    <h1>Things worth celebrating <span class="script">about you</span></h1>

    <div class="card">
      <div class="reason">
        <span class="number">1</span>
        <span>Your strength — you keep learning and trying.</span>
      </div>
      <div class="reason">
        <span class="number">2</span>
        <span>Your kindness — small acts can mean so much.</span>
      </div>
      <div class="reason">
        <span class="number">3</span>
        <span>Your uniqueness — nobody else is exactly you.</span>
      </div>
      <div class="reason">
        <span class="number">4</span>
        <span>Your dreams — they're worth taking one step at a time.</span>
      </div>
      <div class="reason">
        <span class="number">5</span>
        <span>Your presence — you matter, even on ordinary days.</span>
      </div>
    </div>

    <p class="subtitle">A reminder, not a test. You don't have to prove your worth. ♡</p>
    <button class="btn" onclick="goTo('boost')">Tap for a confidence boost</button>
    <button class="btn secondary" onclick="goTo('letterPage')">← Read the letter</button>
  </section>

  <!-- PAGE 4: CONFIDENCE BOOST -->
  <section class="screen" id="boost">
    <div class="eyebrow">Your little confidence corner</div>
    <div class="big-heart">💖</div>
    <h1 class="script">You've got this, meee!</h1>

    <div class="card" style="text-align:center">
      <p id="quote" style="font-size:19px;line-height:1.8">
        One small step is still progress.
      </p>
      <div class="meter"><span id="meterFill"></span></div>
      <p class="small">A little reminder for whenever you need one.</p>
      <button class="btn" onclick="newQuote()">Another reminder ↻</button>
    </div>

    <button class="btn" onclick="celebrate()">Send some confetti!</button>
    <button class="btn secondary" onclick="goTo('final')">One last thing ♡</button>
  </section>

  <!-- PAGE 5: ENDING -->
  <section class="screen" id="final">
    <div class="eyebrow">One last reminder</div>
    <div class="big-heart">🌷</div>
    <h1>Dear meee,<br><span class="script">keep being you.</span></h1>

    <p class="subtitle">
      You don't need to have everything figured out.
      Keep growing, keep dreaming, and remember
      to give yourself the same kindness you give others.
    </p>

    <div class="card" style="text-align:center">
      <p style="font-size:19px;font-weight:800">
        Tum bhot strong ho.<br>
        Tum sab kar sakti ho. ♡
      </p>
      <p>One day at a time. One step at a time.</p>
      <p class="script">You're doing better than you think.</p>
    </div>

    <button class="btn" onclick="celebrate()">Celebrate you! 🎉</button>
    <button class="btn secondary" onclick="goTo('home')">Read it all again ↺</button>

    <footer>This little website is your reminder to be kind to yourself. ♡</footer>
  </section>

</main>

<script>
const screens = document.querySelectorAll('.screen');

function goTo(id) {
  screens.forEach(screen => screen.classList.remove('active'));
  document.getElementById(id).classList.add('active');
  window.scrollTo({ top: 0, behavior: 'smooth' });

  if (id === 'boost') {
    setTimeout(() => {
      document.getElementById('meterFill').style.width = '100%';
    }, 100);
  }
}

function openLetter() {
  goTo('letterPage');
  celebrate();
}

const quotes = [
  "Tum bhot strong ho. Tum sab kar sakti ho. ♡",
  "You can learn things one step at a time.",
  "Your pace is valid. Keep going gently.",
  "You don't need to be perfect to be amazing.",
  "Small progress is still progress.",
  "Believe in yourself, especially on the hard days.",
  "You deserve the same kindness you give others.",
  "Resting is okay. Starting again is okay too."
];

let quoteIndex = 0;

function newQuote() {
  quoteIndex = (quoteIndex + 1) % quotes.length;
  document.getElementById('quote').textContent = quotes[quoteIndex];
  document.getElementById('meterFill').style.width =
    (30 + quoteIndex * 10) + '%';
}

function celebrate() {
  const symbols = ['💖', '✨', '🌸', '💜', '⭐', '💕', '🎉'];

  for (let i = 0; i < 32; i++) {
    const item = document.createElement('span');
    item.className = 'star';
    item.textContent = symbols[Math.floor(Math.random() * symbols.length)];
    item.style.left = Math.random() * 100 + 'vw';
    item.style.animationDuration = (2 + Math.random() * 3) + 's';
    item.style.fontSize = (14 + Math.random() * 18) + 'px';
    document.body.appendChild(item);

    setTimeout(() => item.remove(), 5200);
  }
}
</script>
</body>
</html>
