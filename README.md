<!DOCTYPE html>
<html lang="zh-Hant">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>My Personal Website</title>

  <!-- Google Font -->
  <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@400;700&family=Noto+Sans+TC:wght@300;400;500&display=swap" rel="stylesheet">

  <style>
    *{
      margin:0;
      padding:0;
      box-sizing:border-box;
    }

    body{
      font-family:'Noto Sans TC', sans-serif;
      color:#fff;
      background:#f5f5f5;
      overflow-x:hidden;
    }

    a{
      text-decoration:none;
    }

    /* Navbar */
    nav{
      position:fixed;
      top:0;
      width:100%;
      padding:20px 60px;
      display:flex;
      justify-content:space-between;
      align-items:center;
      z-index:1000;
      background:rgba(0,0,0,0.25);
      backdrop-filter:blur(5px);
    }

    nav .logo{
      font-size:28px;
      font-weight:bold;
      font-family:'Playfair Display', serif;
      color:white;
    }

    nav ul{
      display:flex;
      gap:30px;
      list-style:none;
    }

    nav ul li a{
      color:white;
      font-size:14px;
      letter-spacing:1px;
      transition:0.3s;
    }

    nav ul li a:hover{
      color:#f3b3b3;
    }

    /* Hero Section */
    .hero{
      height:100vh;
      background:
        linear-gradient(rgba(0,0,0,0.35), rgba(0,0,0,0.35)),
        url('me.jpg') center/cover no-repeat;
      display:flex;
      justify-content:center;
      align-items:center;
      text-align:center;
      padding:20px;
    }

    .hero-content h3{
      font-size:28px;
      margin-bottom:20px;
      font-weight:300;
      color:#f1dede;
    }

    .hero-content h1{
      font-size:72px;
      line-height:1.2;
      font-family:'Playfair Display', serif;
      margin-bottom:30px;
    }

    .btn{
      display:inline-block;
      padding:14px 38px;
      background:#d99c9c;
      color:white;
      border-radius:4px;
      transition:0.3s;
      font-weight:500;
    }

    .btn:hover{
      background:#c98787;
    }

    /* About */
    .section{
      padding:100px 20px;
      background:white;
      color:#333;
    }

    .container{
      max-width:1100px;
      margin:auto;
    }

    .section-title{
      text-align:center;
      margin-bottom:60px;
    }

    .section-title h2{
      font-size:52px;
      font-family:'Playfair Display', serif;
      color:#c98d8d;
      margin-bottom:10px;
    }

    .section-title p{
      color:#777;
      font-size:18px;
    }

    .about{
      display:grid;
      grid-template-columns:1fr 1fr;
      gap:50px;
      align-items:center;
    }

    .about img{
      width:100%;
      border-radius:10px;
      box-shadow:0 10px 30px rgba(0,0,0,0.15);
    }

    .about-text h3{
      font-size:36px;
      margin-bottom:20px;
      font-family:'Playfair Display', serif;
    }

    .about-text p{
      line-height:1.8;
      color:#555;
      margin-bottom:20px;
    }

    /* Portfolio */
    .portfolio{
      background:#f9f5f5;
      text-align:center;
    }

    .work-box{
      background:white;
      padding:50px;
      border-radius:12px;
      box-shadow:0 10px 30px rgba(0,0,0,0.08);
      max-width:700px;
      margin:auto;
    }

    .work-box h3{
      font-size:36px;
      margin-bottom:20px;
      font-family:'Playfair Display', serif;
      color:#444;
    }

    .work-box p{
      color:#666;
      margin-bottom:30px;
      line-height:1.7;
    }

    /* Footer */
    footer{
      background:#222;
      color:#aaa;
      text-align:center;
      padding:30px 20px;
      font-size:14px;
    }

    /* Responsive */
    @media(max-width:768px){

      nav{
        padding:20px;
      }

      nav ul{
        gap:15px;
      }

      .hero-content h1{
        font-size:42px;
      }

      .hero-content h3{
        font-size:20px;
      }

      .about{
        grid-template-columns:1fr;
      }

      .section-title h2{
        font-size:38px;
      }
    }
  </style>
</head>

<body>

  <!-- Navbar -->
  <nav>
    <div class="logo">MyLife</div>

    <ul>
      <li><a href="#home">首頁</a></li>
      <li><a href="#about">關於我</a></li>
      <li><a href="#work">作品集</a></li>
    </ul>
  </nav>

  <!-- Hero -->
  <section class="hero" id="home">
    <div class="hero-content">
      <h3>Welcome to my personal website</h3>

      <h1>
        我熱愛設計<br>
        與創作
      </h1>

      <a href="#work" class="btn">查看作品</a>
    </div>
  </section>

  <!-- About -->
  <section class="section" id="about">
    <div class="container">

      <div class="section-title">
        <h2>About Me</h2>
        <p>簡單介紹一下自己</p>
      </div>

      <div class="about">

        <div>
          <img src="me.jpg" alt="我的照片">
        </div>

        <div class="about-text">
          <h3>Hello!</h3>

          <p>
            你好，我是一位熱愛設計與創作的個人工作者，
            喜歡簡約、優雅且具有情感的視覺風格。
          </p>

          <p>
            這個網站展示了我的個人作品與簡介，
            希望能透過作品傳達我的理念與風格。
          </p>

          <a href="work.pdf" class="btn" target="_blank">
            開啟作品 PDF
          </a>
        </div>

      </div>
    </div>
  </section>

  <!-- Portfolio -->
  <section class="section portfolio" id="work">
    <div class="container">

      <div class="section-title">
        <h2>My Works</h2>
        <p>個人作品展示</p>
      </div>

      <div class="work-box">
        <h3>作品集 PDF</h3>

        <p>
          點擊下方按鈕即可瀏覽我的完整作品集，
          內容包含設計、專案與創作作品。
        </p>

        <a href="work.pdf" class="btn" target="_blank">
          下載 / 開啟作品集
        </a>
      </div>

    </div>
  </section>

  <!-- Footer -->
  <footer>
    © 2025 My Personal Website. All Rights Reserved.
  </footer>

</body>
</html>
