<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Maria · Kopi Bubuk</title>
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:ital,wght@0,400;0,700;1,700&family=Inter:opsz,wght@14..32,400;14..32,600;14..32,700&display=swap" rel="stylesheet">
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      min-height: 100vh;
      display: flex;
      justify-content: center;
      align-items: center;
      background: #3e2b1a;
      font-family: 'Inter', sans-serif;
      padding: 20px;
    }

    .coffee-card {
      max-width: 720px;
      width: 100%;
      background: #fcf6ed;
      border-radius: 48px 48px 32px 32px;
      padding: 2.5rem 2rem 2.8rem;
      box-shadow: 0 20px 40px rgba(0, 0, 0, 0.6), 0 0 0 2px #d9c8b4 inset;
      transition: all 0.2s ease;
      border: 1px solid #b3927a;
      text-align: center;
      position: relative;
    }

    .official-tag {
      display: inline-block;
      background: #1f2a2f;
      color: #efe6d8;
      font-weight: 700;
      font-size: 0.85rem;
      letter-spacing: 2px;
      padding: 0.4rem 1.8rem;
      border-radius: 40px;
      text-transform: uppercase;
      margin-bottom: 1.8rem;
      border: 1px solid #b7a085;
      box-shadow: 0 2px 0 #0f0f0f;
    }

    .brand-name {
      font-family: 'Playfair Display', serif;
      font-size: 4.8rem;
      font-weight: 700;
      letter-spacing: 4px;
      color: #2c1e12;
      line-height: 1;
      margin-bottom: 0.4rem;
      text-shadow: 2px 2px 0 rgba(180, 130, 80, 0.2);
      word-break: break-word;
    }

    .special-coffee {
      font-family: 'Playfair Display', serif;
      font-weight: 700;
      font-size: 1.9rem;
      letter-spacing: 6px;
      color: #4d3220;
      text-transform: uppercase;
      border-top: 2px solid #b3927a;
      border-bottom: 2px solid #b3927a;
      display: inline-block;
      padding: 0.2rem 1.5rem;
      margin-bottom: 1.2rem;
      background: rgba(235, 215, 190, 0.2);
      backdrop-filter: blur(2px);
    }

    .product-details {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      align-items: center;
      gap: 1.2rem 2.5rem;
      margin: 1.5rem 0 1rem;
    }

    .detail-item {
      display: flex;
      flex-direction: column;
      align-items: center;
    }

    .detail-label {
      font-size: 0.7rem;
      letter-spacing: 2px;
      text-transform: uppercase;
      color: #6b4f36;
      font-weight: 600;
      background: #e8d9c8;
      padding: 0.2rem 0.8rem;
      border-radius: 20px;
    }

    .detail-value {
      font-family: 'Playfair Display', serif;
      font-weight: 700;
      font-size: 2.2rem;
      color: #2c1e12;
      line-height: 1.3;
      letter-spacing: 1px;
    }

    .badge-100 {
      background: #9f7b5c;
      color: #fcf3e6;
      padding: 0.25rem 1.4rem;
      border-radius: 40px;
      font-weight: 700;
      font-size: 1.5rem;
      letter-spacing: 3px;
      display: inline-block;
      margin: 0.8rem 0 1.2rem;
      box-shadow: 0 3px 0 #4e3522;
      border: 1px solid #c7ab91;
      font-family: 'Playfair Display', serif;
    }

    .murni-badge {
      font-family: 'Playfair Display', serif;
      font-weight: 700;
      font-size: 2.2rem;
      letter-spacing: 10px;
      color: #3d2b1b;
      background: #e1cdb5;
      padding: 0.1rem 1rem;
      border-radius: 40px;
      display: inline-block;
      border: 1px solid #b3927a;
      box-shadow: inset 0 1px 4px rgba(255, 255, 255, 0.5);
      margin: 0.5rem 0 1rem;
    }

    .sub-brand {
      font-family: 'Playfair Display', serif;
      font-size: 1.6rem;
      font-weight: 700;
      color: #5d3f2a;
      letter-spacing: 6px;
      border-top: 2px dashed #b3927a;
      border-bottom: 2px dashed #b3927a;
      display: inline-block;
      padding: 0.2rem 2rem;
      margin-top: 0.8rem;
      background: rgba(225, 205, 180, 0.2);
    }

    .kopi-bubuk-line {
      display: flex;
      justify-content: center;
      align-items: center;
      gap: 0.6rem;
      flex-wrap: wrap;
      margin: 0.2rem 0;
    }

    .kopi-bubuk-line span {
      font-size: 1.8rem;
      font-weight: 700;
      color: #3d2b1b;
      letter-spacing: 4px;
      text-transform: uppercase;
    }

    .robusta {
      font-family: 'Playfair Display', serif;
      font-weight: 700;
      font-size: 2.2rem;
      color: #3d2b1b;
      letter-spacing: 6px;
      background: #e1cdb5;
      padding: 0.1rem 1.6rem;
      border-radius: 60px;
      display: inline-block;
      border: 1px solid #ac8b72;
      margin: 0.2rem 0;
    }

    .separator-line {
      width: 80px;
      height: 3px;
      background: #b3927a;
      margin: 0.5rem auto;
      border-radius: 10px;
    }

    .agaee {
      font-family: 'Playfair Display', serif;
      font-weight: 700;
      font-size: 2.6rem;
      color: #1f140e;
      letter-spacing: 8px;
      opacity: 0.6;
      margin: 0.2rem 0;
      transform: scaleY(1.2);
      display: inline-block;
      border-bottom: 2px dotted #b3927a;
      padding-bottom: 0.2rem;
    }

    .vintage-stripe {
      background: repeating-linear-gradient(45deg, #dac2ab 0px, #dac2ab 4px, #eee0d1 4px, #eee0d1 8px);
      height: 6px;
      width: 70%;
      margin: 1rem auto 0.6rem;
      border-radius: 20px;
    }

    /* --- GAYA BARU: KONTAK & LOKASI --- */
    .contact-section {
      margin-top: 2rem;
      padding-top: 1.2rem;
      border-top: 2px solid #dac2ab;
      display: flex;
      flex-direction: column;
      align-items: center;
      gap: 0.8rem;
    }

    .contact-item {
      display: flex;
      align-items: center;
      justify-content: center;
      flex-wrap: wrap;
      gap: 0.5rem 0.8rem;
      font-size: 0.95rem;
      color: #2c1e12;
      background: rgba(225, 205, 180, 0.25);
      padding: 0.4rem 1.2rem;
      border-radius: 40px;
      border: 1px solid #b3927a;
      width: fit-content;
      backdrop-filter: blur(2px);
    }

    .contact-item .label {
      font-weight: 600;
      letter-spacing: 1px;
      color: #5d3f2a;
      font-size: 0.7rem;
      text-transform: uppercase;
      background: #e8d9c8;
      padding: 0.15rem 0.8rem;
      border-radius: 20px;
    }

    .contact-item .value {
      font-weight: 600;
      letter-spacing: 0.3px;
      word-break: break-word;
    }

    .contact-item .value a {
      color: #2c1e12;
      text-decoration: none;
      border-bottom: 1px dotted #b3927a;
    }

    .contact-item .value a:hover {
      border-bottom: 2px solid #7a5d44;
    }

    /* responsive */
    @media (max-width: 500px) {
      .coffee-card {
        padding: 1.8rem 1.2rem;
        border-radius: 32px;
      }
      .brand-name { font-size: 3.6rem; }
      .special-coffee { font-size: 1.3rem; letter-spacing: 4px; padding: 0.1rem 0.8rem; }
      .detail-value { font-size: 1.6rem; }
      .badge-100 { font-size: 1.2rem; padding: 0.15rem 1rem; }
      .murni-badge { font-size: 1.8rem; letter-spacing: 6px; }
      .robusta { font-size: 1.6rem; padding: 0.05rem 1rem; }
      .sub-brand { font-size: 1.2rem; letter-spacing: 4px; padding: 0.1rem 1rem; }
      .agaee { font-size: 2rem; letter-spacing: 4px; }
      .contact-item { font-size: 0.85rem; padding: 0.3rem 1rem; }
    }

    @media (max-width: 380px) {
      .brand-name { font-size: 2.8rem; }
      .special-coffee { font-size: 1rem; letter-spacing: 2px; }
    }
  </style>
</head>
<body>
  <div class="coffee-card">

    <!-- OFFICIAL TAG -->
    <div class="official-tag">✦ OFFICIAL ✦</div>

    <!-- NAMA MARIA -->
    <h1 class="brand-name">maria</h1>

    <!-- SPECIAL COFFEE -->
    <div class="special-coffee">SPECIALCOFFEE</div>

    <!-- detail produk -->
    <div class="product-details">
      <div class="detail-item">
        <span class="detail-label">jenis</span>
        <span class="detail-value">KOPI <span style="font-weight:400;">BUBUK</span></span>
      </div>
      <div class="detail-item">
        <span class="detail-label">varietas</span>
        <span class="detail-value">ROBUSTA</span>
      </div>
    </div>

    <div class="separator-line"></div>

    <!-- 100% MURNI -->
    <div style="display: flex; justify-content: center; align-items: center; gap: 0.6rem; flex-wrap: wrap; margin: 0.2rem 0;">
      <span class="badge-100">100%</span>
      <span class="murni-badge">MURNI</span>
    </div>

    <div class="agaee">Agaee</div>
    <div class="sub-brand">AgaestORE</div>

    <div class="vintage-stripe"></div>

    <!-- aksen kopi bubuk & robusta -->
    <div class="kopi-bubuk-line" style="margin-top: 0.4rem;">
      <span>✦</span>
      <span>KOPI BUBUK</span>
      <span>✦</span>
    </div>
    <div class="robusta" style="margin-top: 0.2rem;">ROBUSTA</div>

    <!-- watermark kecil -->
    <div style="margin-top: 1.2rem; opacity: 0.5; font-size: 0.8rem; letter-spacing: 3px; color: #4d3220; border-top: 1px solid #dac2ab; padding-top: 0.8rem; font-weight: 600;">
      <span>✦ 100% MURNI ✦</span>
    </div>

    <!-- ===== BAGIAN KONTAK & LOKASI (BARU) ===== -->
    <div class="contact-section">
      <!-- lokasi -->
      <div class="contact-item">
        <span class="label">📍 lokasi</span>
        <span class="value">SMA 15, Jakarta</span>
      </div>
      <!-- email -->
      <div class="contact-item">
        <span class="label">✉️ email</span>
        <span class="value"><a href="mailto:sma15jakarta@gmail.com">sma15jakarta@gmail.com</a></span>
      </div>
      <!-- telepon -->
      <div class="contact-item">
        <span class="label">📞 telepon</span>
        <span class="value"><a href="tel:+628123456788">0812 3456 788</a></span>
      </div>
    </div>

  </div>9
</body>l c.      
</html>ĺm4lmmn
