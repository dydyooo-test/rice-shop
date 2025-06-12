<!DOCTYPE html>
<html lang="ja">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>こだわり米処 ふじい</title>
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link href="https://fonts.googleapis.com/css2?family=Noto+Serif+JP:wght@500;700&display=swap" rel="stylesheet">
  <style>
    body {
      margin: 0;
      font-family: 'Noto Serif JP', serif;
      background-color: #faf8f5;
      color: #333;
    }
    header {
      background-color: #fff;
      padding: 20px 40px;
      box-shadow: 0 2px 8px rgba(0,0,0,0.1);
      display: flex;
      justify-content: space-between;
      align-items: center;
    }
    header h1 {
      margin: 0;
      font-size: 1.8em;
    }
    nav a {
      margin-left: 20px;
      text-decoration: none;
      color: #3b3b3b;
      font-weight: bold;
    }
    .hero {
      background: url('https://images.unsplash.com/photo-1607189200598-62c5952d10f7') center/cover no-repeat;
      height: 60vh;
      display: flex;
      align-items: center;
      justify-content: center;
      color: white;
      text-shadow: 1px 1px 4px #000;
    }
    .hero h2 {
      font-size: 3em;
    }
    section {
      padding: 60px 20px;
      max-width: 1000px;
      margin: auto;
    }
    .about, .products, .contact {
      margin-bottom: 60px;
    }
    .products-list {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 30px;
    }
    .product-item {
      background: #fff;
      border-radius: 8px;
      box-shadow: 0 4px 8px rgba(0,0,0,0.1);
      overflow: hidden;
      transition: transform 0.3s;
    }
    .product-item:hover {
      transform: translateY(-5px);
    }
    .product-item img {
      width: 100%;
      height: 180px;
      object-fit: cover;
    }
    .product-info {
      padding: 15px;
    }
    footer {
      background-color: #3b3b3b;
      color: #fff;
      text-align: center;
      padding: 20px;
    }
  </style>
</head>
<body>
  <header>
    <h1>こだわり米処 ふじい</h1>
    <nav>
      <a href="#about">当店について</a>
      <a href="#products">商品一覧</a>
      <a href="#contact">お問い合わせ</a>
    </nav>
  </header>

  <div class="hero">
    <h2>日本の心、お米をあなたに。</h2>
  </div>

  <section class="about" id="about">
    <h2>当店について</h2>
    <p>
      「こだわり米処 ふじい」は、新潟や秋田の契約農家から厳選したお米のみを扱う専門店です。
      精米から配送まで、鮮度にこだわった美味しいお米を全国にお届けします。
    </p>
  </section>

  <section class="products" id="products">
    <h2>商品一覧</h2>
    <div class="products-list">
      <div class="product-item">
        <img src="https://images.unsplash.com/photo-1611279933602-df1e1cb11d7b" alt="コシヒカリ">
        <div class="product-info">
          <h3>新潟産コシヒカリ（5kg）</h3>
          <p>粘りと甘みのバランスが絶妙。人気No.1。</p>
        </div>
      </div>
      <div class="product-item">
        <img src="https://images.unsplash.com/photo-1591035897813-30a5a8121d41" alt="あきたこまち">
        <div class="product-info">
          <h3>秋田産あきたこまち（5kg）</h3>
          <p>あっさりした口当たりで、毎日の食卓に。</p>
        </div>
      </div>
      <div class="product-item">
        <img src="https://images.unsplash.com/photo-1622782269736-3be1f82fb1c6" alt="玄米">
        <div class="product-info">
          <h3>北海道産有機玄米（5kg）</h3>
          <p>健康志向のあなたへ、安心のオーガニック。</p>
        </div>
      </div>
    </div>
  </section>

  <section class="contact" id="contact">
    <h2>お問い合わせ</h2>
    <p>ご注文・ご質問は以下のメールアドレスまでご連絡ください。</p>
    <p><strong>Email:</strong> info@fujii-rice.jp</p>
  </section>

  <footer>
    <p>&copy; 2025 こだわり米処 ふじい. All rights reserved.</p>
  </footer>

  <script>
    // スムーズスクロール（クリックで移動）
    document.querySelectorAll('nav a').forEach(anchor => {
      anchor.addEventListener('click', function(e) {
        e.preventDefault();
        document.querySelector(this.getAttribute('href')).scrollIntoView({
          behavior: 'smooth'
        });
      });
    });
  </script>
</body>
</html>
