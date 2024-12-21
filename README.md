<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Happy Birthday</title>
  <style>
    body {
      margin: 0;
      padding: 0;
      background: linear-gradient(135deg, #ff9a9e, #fad0c4);
      font-family: 'Comic Sans MS', cursive, sans-serif;
      min-height: 100vh;
      overflow-y: auto; /* Izinkan scroll */
      position: relative;
    }
    #button {
      padding: 15px 30px;
      font-size: 20px;
      background-color: #ff007f;
      color: white;
      border: none;
      border-radius: 15px;
      cursor: pointer;
      box-shadow: 0 5px 10px rgba(0, 0, 0, 0.3);
      transition: transform 0.3s ease, box-shadow 0.3s ease, background-color 0.3s ease;
    }
    #button:hover {
      transform: scale(1.1);
      background-color: #d8006e;
      box-shadow: 0 8px 15px rgba(0, 0, 0, 0.5);
    }
    #button:active {
      transform: scale(0.95);
      background-color: #b0005b;
    }
    #message {
      display: none;
      text-align: center;
      color: white;
      font-size: 24px;
      background: rgba(0, 0, 0, 0.7);
      padding: 20px;
      border-radius: 15px;
      margin: 20px auto;
      max-width: 600px;
    }
    .balloon {
      position: fixed;
      bottom: -100px;
      border-radius: 50%;
      animation: rise 6s infinite ease-in-out;
    }
    .sparkle {
      position: absolute;
      width: 10px;
      height: 10px;
      background: radial-gradient(circle, rgba(255, 255, 255, 0.9), transparent);
      border-radius: 50%;
      animation: sparkle 1s ease-out infinite, twinkle 1.5s infinite;
    }
    @keyframes rise {
      0% {
        transform: translateY(0) scale(1);
        opacity: 1;
      }
      100% {
        transform: translateY(-110vh) scale(1.2);
        opacity: 0.5;
      }
    }
    @keyframes sparkle {
      0% {
        transform: scale(0.5);
        opacity: 1;
      }
      100% {
        transform: scale(2);
        opacity: 0;
      }
    }
    @keyframes twinkle {
      0%, 100% {
        opacity: 1;
      }
      50% {
        opacity: 0.5;
      }
    }
  </style>
</head>
<body>
  <div style="text-align: center; padding-top: 50px;">
    <button id="button">Coba pencet</button>
    <div id="message">
        <h1>Haalllooo Sayangggkuu Tersayang Bangetttt!!!!</h1>
        <p>
          Selamat ulang tahunn yaaa cinta hatiku yang paaling manis, cantik, imut, lucuuu, gemess, menggemparkan duniaku, pokoknya kesayangan aku dunia akhirattt! 🎉💖💘<br><br>
      
          Di hari spesial kamu ini, aku cuma mau bilang kalau aku tuh sayanggg bangettt sama kamuuu, sampe rasanya hati aku nggak cukup buat nampung semua rasa cinta aku ke kamu ❤💞. Kamu tuh kayak pelangi abis hujan, kayak bunga yang mekar di musim semi, pokoknya kamuuu indahhh banget di mata aku! 🌈🌸<br><br>
      
          Setiap hari, aku bersyukur banget bisa kenal kamu, bisa punya kamu, dan bisa jadi bagian kecil dari hidup kamu. Kamu itu ibarat matahari buat aku, yang selalu bikin hariku lebih cerah dan hangat ☀✨. Tanpa kamu, hidup aku bakal kayak malam tanpa bintang, kosonggg banget 😢.<br><br>
      
          Aku doain yaaa di ulang tahun kamu ini, semua harapan kamu terkabul! Semoga kamu selalu sehat, bahagia, panjang umur, makin cantik luar dalam, makin sukses, dan semoga kamu juga makin sayang sama aku hehehe 😘💋. Aku pengen kita selalu bareng-bareng, jalanin hari-hari penuh kebahagiaan dan cinta, karena aku nggak pernah bisa bayangin hidup aku tanpa kamuuu ❤💖.<br><br>
      
          Tau nggak? Aku tuh tiap malam selalu mikirin kamu, tiap bangun pagi yang pertama kali aku inget tuh kamuuu! 😍❤ Kamu tuh kayak canduuuuu buat aku, yang nggak pernah bikin aku bosen! Aku sayang banget sama kamu, sampe rasanya pengen teriak ke seluruh dunia kalau aku cinta kamu seumur hidup aku!!! 🌍💌<br><br>
      
          Jadi, di hari spesial kamu ini, aku cuma mau bilang... terima kasih banget karena kamu udah jadi bagian paling penting dalam hidup aku. Kamu itu nggak cuma pacar aku, tapi juga sahabat aku, partner aku, dan belahan jiwa aku 💖💞. Aku nggak sabar buat ngerayain lebih banyak ulang tahun kamu di tahun-tahun yang akan datang! 🎂🥳<br><br>
      
          Pokoknya kamu itu segalanya buat aku. Dari ujung rambut sampe ujung kaki, aku cinta banget sama kamuuu ❤❤❤. Jangan pernah ragu ya, aku akan selalu ada buat kamu, di saat senang atau sedih, aku bakal terus ada di samping kamu selamanya! 💕💍<br><br>
      
          Selamat ulang tahun yaa sayangggku tercintahhh, semoga kamu makin bahagiaaa hari ini dan selaluaa!! Aku cinta kamu lebih dari yang kata-kata bisa gambarkan! Love you to the moon and back, infinity and beyond!!! 😘💖💋<br><br>
      
          Peluk paling hangat dan cium paling manis dari aku buat kamuuu,<br>
          ~ Dari Aku yang Paling Sayang Kamu, Selamanya- kak ian ~ ❤❤❤
        </p>
      </div>
  </div>

  <script>
    const button = document.getElementById('button');
    const message = document.getElementById('message');

    button.addEventListener('click', () => {
      message.style.display = 'block';
      generateBalloons(100); // Tambahkan lebih banyak balon
      generateSparkles(350); // Tambahkan lebih banyak sprinkle
    });

    function generateBalloons(count) {
      for (let i = 0; i < count; i++) {
        const balloon = document.createElement('div');
        balloon.classList.add('balloon');
        balloon.style.width = `${Math.random() * 30 + 20}px`;
        balloon.style.height = `${Math.random() * 50 + 30}px`;
        balloon.style.left = `${Math.random() * 100}vw`;
        balloon.style.background = `hsl(${Math.random() * 360}, 80%, 60%)`;
        balloon.style.animationDelay = `${Math.random() * 2}s`;
        document.body.appendChild(balloon);

        setTimeout(() => {
          balloon.remove();
        }, 6000);
      }
    }

    function generateSparkles(count) {
      for (let i = 0; i < count; i++) {
        const sparkle = document.createElement('div');
        sparkle.classList.add('sparkle');
        sparkle.style.left = `${Math.random() * 100}vw`;
        sparkle.style.top = `${Math.random() * 100}vh`;
        sparkle.style.background = `hsl(${Math.random() * 360}, 80%, 90%)`;
        sparkle.style.animationDelay = `${Math.random() * 1.5}s`;
        document.body.appendChild(sparkle);

        setTimeout(() => {
          sparkle.remove();
        }, 1500);
      }
    }
  </script>
</body>
</html>
