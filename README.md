# Teste-3
<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Empório da Pamonha | Jardim D'Icaraí, Salto - SP</title>
<meta name="description" content="Pamonha na palha, quentinha e feita na hora. Peça agora e receba em Jardim D'Icaraí, Salto - SP.">
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Fraunces:ital,opsz,wght@0,9..144,400;0,9..144,600;0,9..144,700;0,9..144,900;1,9..144,500;1,9..144,600&family=Work+Sans:wght@400;500;600;700&family=Caveat:wght@600;700&display=swap" rel="stylesheet">
<style>
  :root{
    --cream: #F5EFD6;
    --paper: #FFFCF2;
    --ink: #2B2116;
    --ink-soft: #5A4E3B;
    --husk: #566B37;
    --husk-dark: #34401F;
    --corn: #F0AD2E;
    --corn-soft: #F8D485;
    --ember: #B23A1F;
    --ember-dark: #8B2C16;
    --line: rgba(43,33,22,0.14);
  }
  *{box-sizing:border-box;margin:0;padding:0;}
  html{scroll-behavior:smooth;}
  body{
    background:var(--cream);
    background-image:
      radial-gradient(circle at 1px 1px, rgba(43,33,22,0.05) 1px, transparent 0);
    background-size:18px 18px;
    color:var(--ink);
    font-family:'Work Sans',sans-serif;
    line-height:1.5;
    -webkit-font-smoothing:antialiased;
    padding-bottom:0;
  }
  img{max-width:100%;display:block;}
  a{text-decoration:none;color:inherit;}
  .wrap{max-width:1160px;margin:0 auto;padding:0 24px;}
  h1,h2,h3{font-family:'Fraunces',serif;color:var(--ink);letter-spacing:-0.01em;}
  em{font-style:italic;}
  .icon{width:22px;height:22px;stroke:currentColor;fill:none;stroke-width:1.8;stroke-linecap:round;stroke-linejoin:round;flex-shrink:0;}

  @media (prefers-reduced-motion: reduce){
    *{animation:none !important;transition:none !important;}
  }

  ::-webkit-scrollbar{display:none;}
  .no-scrollbar{scrollbar-width:none;-ms-overflow-style:none;}

  /* ---------- NAV ---------- */
  .nav{
    position:sticky;top:0;z-index:60;
    background:rgba(245,239,214,0.9);
    backdrop-filter:blur(8px);
    border-bottom:1px solid var(--line);
  }
  .nav-inner{
    display:flex;align-items:center;justify-content:space-between;
    padding:14px 24px;
  }
  .brand{
    font-family:'Fraunces',serif;font-weight:700;font-size:1.1rem;
    color:var(--husk-dark);
    display:flex;align-items:center;gap:8px;
  }
  .brand b{color:var(--ember);font-weight:700;}

  .btn{
    display:inline-flex;align-items:center;gap:8px;
    background:var(--ember);color:#fff;
    font-weight:600;font-size:0.95rem;font-family:'Work Sans',sans-serif;
    padding:13px 24px;border-radius:100px;
    border:none;cursor:pointer;
    transition:transform .15s ease, background .2s ease, box-shadow .2s ease;
    box-shadow:0 6px 18px rgba(178,58,31,0.32);
    white-space:nowrap;
  }
  .btn:hover{background:var(--ember-dark);transform:translateY(-2px);box-shadow:0 10px 22px rgba(178,58,31,0.4);}
  .btn:focus-visible{outline:3px solid var(--corn);outline-offset:2px;}
  .btn-sm{padding:10px 18px;font-size:0.85rem;}
  .btn-corn{background:var(--corn);color:var(--ink);box-shadow:0 6px 18px rgba(240,173,46,0.35);}
  .btn-corn:hover{background:var(--corn-soft);color:var(--ink);}

  /* ---------- HERO ---------- */
  .hero{
    position:relative;
    min-height:88vh;
    display:flex;align-items:flex-end;
    overflow:hidden;
    isolation:isolate;
  }
  .hero-bg{
    position:absolute;inset:0;z-index:-2;
    background-image:url('https://images.brendi.com.br/optimized/ca88b94deb37769f8154696a9617b7d8');
    background-size:cover;background-position:center 65%;
  }
  .hero-scrim{
    position:absolute;inset:0;z-index:-1;
    background:linear-gradient(180deg, rgba(30,22,13,0.25) 0%, rgba(30,22,13,0.55) 45%, rgba(24,18,10,0.94) 100%);
  }
  .steam{
    position:absolute;border-radius:50%;
    background:radial-gradient(closest-side, rgba(255,255,255,0.5), transparent 70%);
    filter:blur(6px);
    opacity:0;
  }
  .steam-1{width:90px;height:140px;top:12%;left:38%;animation:rise 7s ease-in-out infinite;}
  .steam-2{width:70px;height:110px;top:18%;left:47%;animation:rise 8.5s ease-in-out 1.5s infinite;}
  .steam-3{width:60px;height:100px;top:22%;left:55%;animation:rise 6.5s ease-in-out 3s infinite;}
  @keyframes rise{
    0%{transform:translateY(0) scale(1);opacity:0;}
    20%{opacity:0.35;}
    80%{opacity:0.12;}
    100%{transform:translateY(-70px) scale(1.3);opacity:0;}
  }

  .hero-content{position:relative;padding:64px 0 56px;width:100%;}
  .hero-eyebrow{
    color:var(--corn-soft);font-weight:600;font-size:0.82rem;
    letter-spacing:0.08em;text-transform:uppercase;
    margin-bottom:16px;display:flex;align-items:center;gap:10px;
  }
  .hero-eyebrow::before{content:"";width:26px;height:2px;background:var(--corn);}
  .hero h1{
    color:#FFF9EA;
    font-size:clamp(2.1rem, 6vw, 3.6rem);
    font-weight:700;line-height:1.06;
    max-width:16ch;
    margin-bottom:18px;
    text-wrap:balance;
  }
  .hero h1 em{color:var(--corn-soft);font-weight:500;}
  .hero p.lead{
    color:#EFE6CE;font-size:1.08rem;max-width:42ch;margin-bottom:30px;
  }
  .hero-ctas{display:flex;flex-wrap:wrap;gap:14px;align-items:center;}

  .stamp{
    position:absolute;top:26px;right:24px;z-index:2;
    width:112px;height:112px;border-radius:50%;
    border:2px dashed rgba(255,249,234,0.75);
    display:flex;align-items:center;justify-content:center;
    transform:rotate(10deg);
  }
  .stamp span{
    font-family:'Caveat',cursive;font-weight:700;font-size:1.2rem;
    color:#FFF9EA;text-align:center;line-height:1.05;text-transform:uppercase;
  }

  /* ---------- USP BAR ---------- */
  .usp{background:var(--paper);border-bottom:1px solid var(--line);}
  .usp-inner{
    display:grid;grid-template-columns:repeat(3,1fr);
    padding:26px 0;
  }
  .usp-item{
    display:flex;align-items:center;gap:12px;
    padding:0 20px;
    border-left:1px solid var(--line);
  }
  .usp-item:first-child{border-left:none;}
  .usp-item .icon{color:var(--ember);width:26px;height:26px;}
  .usp-item h3{font-size:0.95rem;font-weight:700;font-family:'Work Sans',sans-serif;color:var(--ink);}
  .usp-item p{font-size:0.8rem;color:var(--ink-soft);}

  /* ---------- CATEGORY CHIPS ---------- */
  .cat-strip{
    display:flex;gap:10px;overflow-x:auto;padding:20px 24px;
    background:var(--cream);
  }
  .cat-chip{
    flex:0 0 auto;
    background:var(--paper);border:1px solid var(--line);
    padding:9px 18px;border-radius:100px;
    font-size:0.85rem;font-weight:600;color:var(--husk-dark);
    transition:background .15s ease, color .15s ease, border-color .15s ease;
  }
  .cat-chip:hover{background:var(--husk-dark);color:#FFF9EA;border-color:var(--husk-dark);}

  /* ---------- SECTIONS ---------- */
  .section{padding:60px 0;}
  .section-head{
    display:flex;justify-content:space-between;align-items:flex-end;gap:20px;
    margin-bottom:30px;flex-wrap:wrap;
  }
  .section-head h2{font-size:clamp(1.5rem,3.2vw,2.1rem);font-weight:700;}
  .section-head p{color:var(--ink-soft);max-width:48ch;font-size:0.97rem;margin-top:6px;}
  .kicker{
    font-size:0.78rem;font-weight:700;letter-spacing:0.06em;text-transform:uppercase;
    color:var(--ember);margin-bottom:8px;display:block;
  }

  /* ---------- CAROUSEL ---------- */
  .carousel{
    display:flex;gap:18px;overflow-x:auto;padding:4px 24px 20px;
    scroll-snap-type:x mandatory;
    margin:0 -24px;
  }
  .carousel .card{scroll-snap-align:start;flex:0 0 220px;}
  @media (min-width:720px){
    .carousel{padding-left:0;padding-right:0;margin:0;}
    .carousel .card{flex:0 0 232px;}
  }

  .card{
    background:var(--paper);
    border-radius:18px;overflow:hidden;border:1px solid var(--line);
    display:flex;flex-direction:column;
    transition:transform .2s ease, box-shadow .2s ease;
  }
  .card:hover{transform:translateY(-6px);box-shadow:0 20px 34px -18px rgba(43,33,22,0.28);}
  .card-media{position:relative;}
  .card-img{width:100%;height:148px;object-fit:cover;}
  .badge{
    position:absolute;top:10px;left:10px;
    background:var(--corn);color:var(--ink);
    font-size:0.65rem;font-weight:700;text-transform:uppercase;letter-spacing:0.04em;
    padding:4px 10px;border-radius:100px;
  }
  .card-body{padding:15px 16px 17px;display:flex;flex-direction:column;gap:6px;flex:1;}
  .card-body h3{font-size:1rem;font-weight:600;line-height:1.25;}
  .card-price{margin-top:auto;display:flex;align-items:center;justify-content:space-between;padding-top:10px;}
  .price{font-family:'Fraunces',serif;font-weight:700;color:var(--husk-dark);font-size:1.12rem;}
  .mini-link{font-size:0.78rem;font-weight:700;color:var(--ember);}

  /* ---------- COMBOS / CUPONS ---------- */
  .combos{background:var(--husk-dark);color:#F3F0DF;padding:64px 0;}
  .combos .section-head h2, .combos .kicker{color:#F3F0DF;}
  .combos .kicker{color:var(--corn-soft);}
  .combos .section-head p{color:#CBD3B7;}

  .coupon-grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(240px,1fr));gap:26px;}
  .coupon{
    position:relative;
    background:rgba(255,252,242,0.06);
    border:2px dashed rgba(243,240,223,0.35);
    border-radius:16px;
    padding:20px 22px 20px 22px;
    display:flex;flex-direction:column;gap:8px;
  }
  .coupon::before,.coupon::after{
    content:"";position:absolute;width:22px;height:22px;
    background:var(--husk-dark);border-radius:50%;
    top:50%;transform:translateY(-50%);
  }
  .coupon::before{left:-11px;}
  .coupon::after{right:-11px;}
  .coupon .serves{font-size:0.72rem;color:var(--corn-soft);font-weight:700;text-transform:uppercase;letter-spacing:0.04em;}
  .coupon h3{color:#FFF9EA;font-size:1.08rem;}
  .coupon p.desc{font-size:0.87rem;color:#D6DBC4;}
  .coupon .price{color:var(--corn-soft);font-size:1.3rem;margin-top:4px;}

  /* ---------- CARDÁPIO ACCORDION ---------- */
  .menu-accordion{display:flex;flex-direction:column;gap:12px;}
  details{
    background:var(--paper);border:1px solid var(--line);border-radius:14px;
    overflow:hidden;
  }
  summary{
    list-style:none;cursor:pointer;
    display:flex;align-items:center;justify-content:space-between;
    padding:18px 20px;font-family:'Fraunces',serif;font-weight:600;font-size:1.05rem;
  }
  summary::-webkit-details-marker{display:none;}
  summary .count{
    font-family:'Work Sans',sans-serif;font-size:0.78rem;font-weight:600;
    color:var(--ink-soft);margin-left:10px;flex:1;
  }
  summary .chev{transition:transform .2s ease;color:var(--ember);}
  details[open] summary .chev{transform:rotate(180deg);}
  .menu-list{padding:0 20px 18px;display:flex;flex-direction:column;gap:12px;}
  .menu-row{display:flex;align-items:baseline;gap:8px;}
  .menu-row .name{font-weight:600;white-space:nowrap;font-size:0.95rem;}
  .menu-row .leader{flex:1;border-bottom:2px dotted var(--line);transform:translateY(-4px);}
  .menu-row .price{font-family:'Fraunces',serif;font-weight:700;white-space:nowrap;color:var(--husk-dark);}
  .tag{font-size:0.62rem;font-weight:700;text-transform:uppercase;padding:2px 7px;border-radius:100px;margin-left:2px;}
  .tag-new{background:var(--corn);color:var(--ink);}
  .tag-diet{background:var(--husk);color:#FFF9EA;}

  /* ---------- FINAL CTA ---------- */
  .final-cta{
    background:var(--ember);color:#fff;border-radius:26px;padding:52px 36px;text-align:center;position:relative;overflow:hidden;
  }
  .final-cta h2{color:#fff;font-size:clamp(1.7rem,4vw,2.5rem);margin-bottom:12px;}
  .final-cta p{color:#FBDCCF;max-width:50ch;margin:0 auto 26px;font-size:1.02rem;}
  .final-cta .btn{background:#FFF9EA;color:var(--ember-dark);}
  .final-cta .btn:hover{background:var(--corn-soft);color:var(--ink);}
  .final-cta small{display:block;margin-top:18px;color:#F4C9B8;font-size:0.78rem;}

  /* ---------- FOOTER ---------- */
  footer{padding:36px 0 100px;color:var(--ink-soft);font-size:0.83rem;border-top:1px solid var(--line);margin-top:20px;}
  .footer-inner{display:flex;justify-content:space-between;flex-wrap:wrap;gap:10px;}

  /* ---------- STICKY MOBILE BAR ---------- */
  .sticky-bar{
    display:none;
    position:fixed;left:0;right:0;bottom:0;z-index:70;
    background:var(--paper);
    border-top:1px solid var(--line);
    box-shadow:0 -10px 24px rgba(43,33,22,0.14);
    padding:12px 16px;
    align-items:center;justify-content:space-between;gap:12px;
  }
  .sticky-bar p{font-size:0.82rem;font-weight:600;color:var(--ink-soft);}
  .sticky-bar strong{display:block;font-family:'Fraunces',serif;font-size:0.95rem;color:var(--ink);}

  @media (max-width:680px){
    .sticky-bar{display:flex;}
    footer{padding-bottom:110px;}
  }

  @media (max-width:900px){
    .usp-inner{grid-template-columns:1fr;gap:14px;}
    .usp-item{border-left:none;border-top:1px solid var(--line);padding-top:14px;}
    .usp-item:first-child{border-top:none;padding-top:0;}
  }
  @media (max-width:520px){
    .final-cta{padding:38px 20px;border-radius:20px;}
    .stamp{width:90px;height:90px;top:16px;right:16px;}
    .stamp span{font-size:1rem;}
  }
</style>
</head>
<body>

<nav class="nav">
  <div class="wrap nav-inner">
    <div class="brand">🌽 EMPÓRIO <b>DA PAMONHA</b></div>
    <a class="btn btn-sm" href="https://pedido.brendi.com.br/emporio-da-pamonha-jardim-dicarai/" target="_blank" rel="noopener">Fazer pedido</a>
  </div>
</nav>

<!-- HERO -->
<header class="hero">
  <div class="hero-bg"></div>
  <div class="hero-scrim"></div>
  <div class="steam steam-1"></div>
  <div class="steam steam-2"></div>
  <div class="steam steam-3"></div>
  <div class="stamp"><span>Feito<br>na hora</span></div>
  <div class="wrap hero-content">
    <div class="hero-eyebrow">Jardim D'Icaraí · Salto, SP</div>
    <h1>Pamonha na palha,<br><em>quentinha</em> e feita na hora.</h1>
    <p class="lead">Direto do milho fresco pra sua mesa — escolha a sua, monte um combo e peça em poucos toques.</p>
    <div class="hero-ctas">
      <a class="btn btn-corn" href="https://pedido.brendi.com.br/emporio-da-pamonha-jardim-dicarai/" target="_blank" rel="noopener">Fazer meu pedido →</a>
    </div>
  </div>
</header>

<!-- USP BAR -->
<section class="usp">
  <div class="wrap usp-inner">
    <div class="usp-item">
      <svg class="icon" viewBox="0 0 24 24"><circle cx="12" cy="12" r="9"/><path d="M12 7v5l3.5 2"/></svg>
      <div><h3>Feito na hora</h3><p>Preparo começa quando o pedido chega</p></div>
    </div>
    <div class="usp-item">
      <svg class="icon" viewBox="0 0 24 24"><path d="M3 16V6a1 1 0 0 1 1-1h9v11"/><path d="M13 9h4l4 4v3h-2"/><circle cx="7.5" cy="17.5" r="1.8"/><circle cx="17.5" cy="17.5" r="1.8"/></svg>
      <div><h3>Entrega rápida</h3><p>Sai quentinho reto pra sua casa</p></div>
    </div>
    <div class="usp-item">
      <svg class="icon" viewBox="0 0 24 24"><path d="M4 8h16l-1.5 11a2 2 0 0 1-2 1.8H7.5a2 2 0 0 1-2-1.8L4 8Z"/><path d="M8 8V6a4 4 0 0 1 8 0v2"/></svg>
      <div><h3>Pedido mínimo R$ 15,00</h3><p>Fácil de fechar o carrinho</p></div>
    </div>
  </div>
</section>

<!-- CATEGORY CHIPS -->
<div class="cat-strip no-scrollbar">
  <a class="cat-chip" href="#cardapio">🌽 Pamonhas</a>
  <a class="cat-chip" href="#cardapio">Chica Bacana</a>
  <a class="cat-chip" href="#cardapio">Bolos de Milho</a>
  <a class="cat-chip" href="#cardapio">Doces</a>
  <a class="cat-chip" href="#cardapio">Sucos</a>
  <a class="cat-chip" href="#cardapio">Bebidas</a>
  <a class="cat-chip" href="#cardapio">Tortas</a>
  <a class="cat-chip" href="#cardapio">Milho Cozido</a>
  <a class="cat-chip" href="#cardapio">Caldo</a>
  <a class="cat-chip" href="#cardapio">Coxinha de Milho</a>
</div>

<!-- MAIS PEDIDOS -->
<section class="section">
  <div class="wrap">
    <div class="section-head">
      <div>
        <span class="kicker">🔥 Os queridinhos</span>
        <h2>Os mais pedidos por aqui</h2>
        <p>Os primeiros a acabar — quem já provou, repete.</p>
      </div>
      <a class="btn btn-sm" style="background:transparent;color:var(--husk-dark);border:1.5px solid var(--husk-dark);box-shadow:none;" href="#cardapio">Ver cardápio completo</a>
    </div>
  </div>
  <div class="carousel no-scrollbar wrap">
    <div class="card">
      <div class="card-media"><img class="card-img" src="https://images.brendi.com.br/optimized/4f60a78e56ec1a888c011efe0c5a12c3" alt="Bolo cremoso assado na palha"></div>
      <div class="card-body"><h3>Bolo cremoso assado na palha</h3>
        <div class="card-price"><span class="price">R$ 40,00</span><span class="mini-link">Pedir →</span></div>
      </div>
    </div>
    <div class="card">
      <div class="card-media"><img class="card-img" src="https://images.brendi.com.br/optimized/4281c99f3d531e0f70c8ecf76142f409" alt="Caldo de milho"></div>
      <div class="card-body"><h3>Caldo de milho</h3>
        <div class="card-price"><span class="price">R$ 25,00</span><span class="mini-link">Pedir →</span></div>
      </div>
    </div>
    <div class="card">
      <div class="card-media"><img class="card-img" src="https://images.brendi.com.br/optimized/449c9a55bcb8c4e1fab10fbc3f95ceed" alt="Pamonha Salgada"></div>
      <div class="card-body"><h3>Pamonha Salgada</h3>
        <div class="card-price"><span class="price">R$ 14,00</span><span class="mini-link">Pedir →</span></div>
      </div>
    </div>
    <div class="card">
      <div class="card-media"><img class="card-img" src="https://images.brendi.com.br/optimized/841ef978a0dbbfb3cc6237149a09d1f2" alt="Pamonha Salgada com Queijo"></div>
      <div class="card-body"><h3>Pamonha Salgada c/ Queijo</h3>
        <div class="card-price"><span class="price">R$ 16,00</span><span class="mini-link">Pedir →</span></div>
      </div>
    </div>
    <div class="card">
      <div class="card-media"><span class="badge">Novidade</span><img class="card-img" src="https://images.brendi.com.br/optimized/ca88b94deb37769f8154696a9617b7d8" alt="Chica Carne Seca"></div>
      <div class="card-body"><h3>Chica Carne Seca</h3>
        <div class="card-price"><span class="price">R$ 22,00</span><span class="mini-link">Pedir →</span></div>
      </div>
    </div>
  </div>
</section>

<!-- COMBOS -->
<section class="combos">
  <div class="wrap">
    <div class="section-head">
      <div>
        <span class="kicker">Combine e economize</span>
        <h2>Compre mais, pague menos</h2>
        <p>Combos pensados pra dividir, repetir ou fechar o dia sem pensar duas vezes.</p>
      </div>
    </div>
    <div class="coupon-grid">
      <div class="coupon">
        <span class="serves">Serve 1 pessoa</span>
        <h3>Chica bacana de frango + Itubaina</h3>
        <p class="desc">Pamonha assada recheada com frango cremoso e catupiry, com uma Itubaina geladinha.</p>
        <span class="price">R$ 25,00</span>
      </div>
      <div class="coupon">
        <span class="serves">Novidade</span>
        <h3>15 Mini Coxinha + Coca 350ml</h3>
        <p class="desc">Coxinhas de massa de milho recheadas com frango, com uma coca gelada de acompanhamento.</p>
        <span class="price">R$ 24,90</span>
      </div>
      <div class="coupon">
        <span class="serves">Leve mais por menos</span>
        <h3>Combo Família</h3>
        <p class="desc">2 pamonhas + 1 curau pelo menor preço — perfeito pra dividir.</p>
        <span class="price">R$ 36,00</span>
      </div>
      <div class="coupon">
        <span class="serves">Leve mais por menos</span>
        <h3>Combo Pamonheiro</h3>
        <p class="desc">3 pamonhas com o menor preço da casa — pra quem não abre mão.</p>
        <span class="price">R$ 39,00</span>
      </div>
    </div>
  </div>
</section>

<!-- CARDÁPIO COMPLETO -->
<section class="section" id="cardapio">
  <div class="wrap">
    <div class="section-head">
      <div>
        <span class="kicker">Cardápio completo</span>
        <h2>Tudo o que sai da nossa cozinha</h2>
        <p>Organizado por categoria — toque para abrir e ver todos os itens e preços.</p>
      </div>
    </div>

    <div class="menu-accordion">
      <details open>
        <summary>Pamonhas <span class="count">7 itens</span> <svg class="icon chev" viewBox="0 0 24 24"><path d="M6 9l6 6 6-6"/></svg></summary>
        <div class="menu-list">
          <div class="menu-row"><span class="name">Pamonha Doce (400g)</span><span class="leader"></span><span class="price">R$ 14,00</span></div>
          <div class="menu-row"><span class="name">Pamonha Salgada (400g)</span><span class="leader"></span><span class="price">R$ 14,00</span></div>
          <div class="menu-row"><span class="name">Pamonha Doce c/ Queijo</span><span class="leader"></span><span class="price">R$ 16,00</span></div>
          <div class="menu-row"><span class="name">Pamonha Salgada c/ Queijo</span><span class="leader"></span><span class="price">R$ 16,00</span></div>
          <div class="menu-row"><span class="name">Pamonha Romeu e Julieta</span><span class="leader"></span><span class="price">R$ 17,00</span></div>
          <div class="menu-row"><span class="name">Pamonha doce com coco</span><span class="leader"></span><span class="price">R$ 14,00</span></div>
          <div class="menu-row"><span class="name">Pamonha da Moda <span class="tag tag-new">Novidade</span></span><span class="leader"></span><span class="price">R$ 18,00</span></div>
        </div>
      </details>

      <details>
        <summary>Chica Bacana <span class="count">3 itens</span> <svg class="icon chev" viewBox="0 0 24 24"><path d="M6 9l6 6 6-6"/></svg></summary>
        <div class="menu-list">
          <div class="menu-row"><span class="name">Chica Carne Seca <span class="tag tag-new">Novidade</span></span><span class="leader"></span><span class="price">R$ 22,00</span></div>
          <div class="menu-row"><span class="name">Chica Frango Catupiry</span><span class="leader"></span><span class="price">R$ 20,00</span></div>
          <div class="menu-row"><span class="name">Chica Calabresa</span><span class="leader"></span><span class="price">R$ 20,00</span></div>
        </div>
      </details>

      <details>
        <summary>Bolos de Milho <span class="count">5 itens</span> <svg class="icon chev" viewBox="0 0 24 24"><path d="M6 9l6 6 6-6"/></svg></summary>
        <div class="menu-list">
          <div class="menu-row"><span class="name">Bolo de milho cremoso</span><span class="leader"></span><span class="price">R$ 35,00</span></div>
          <div class="menu-row"><span class="name">Bolo cremoso assado na palha</span><span class="leader"></span><span class="price">R$ 40,00</span></div>
          <div class="menu-row"><span class="name">Bolo de milho caipira <span class="tag tag-diet">Zero Lactose</span></span><span class="leader"></span><span class="price">R$ 40,00</span></div>
          <div class="menu-row"><span class="name">Bolo Romeu e Julieta (700g)</span><span class="leader"></span><span class="price">R$ 29,00</span></div>
          <div class="menu-row"><span class="name">Bolo de milho individual</span><span class="leader"></span><span class="price">R$ 19,00</span></div>
        </div>
      </details>

      <details>
        <summary>Doces <span class="count">2 itens</span> <svg class="icon chev" viewBox="0 0 24 24"><path d="M6 9l6 6 6-6"/></svg></summary>
        <div class="menu-list">
          <div class="menu-row"><span class="name">Curau (200ml)</span><span class="leader"></span><span class="price">R$ 12,00</span></div>
          <div class="menu-row"><span class="name">Curau na marmitinha (500g)</span><span class="leader"></span><span class="price">R$ 22,00</span></div>
        </div>
      </details>

      <details>
        <summary>Sucos <span class="count">2 itens</span> <svg class="icon chev" viewBox="0 0 24 24"><path d="M6 9l6 6 6-6"/></svg></summary>
        <div class="menu-list">
          <div class="menu-row"><span class="name">Suco de milho verde (300ml)</span><span class="leader"></span><span class="price">R$ 12,00</span></div>
          <div class="menu-row"><span class="name">Suco de milho (1 litro) <span class="tag tag-new">Novidade</span></span><span class="leader"></span><span class="price">R$ 27,00</span></div>
        </div>
      </details>

      <details>
        <summary>Bebidas <span class="count">6 itens</span> <svg class="icon chev" viewBox="0 0 24 24"><path d="M6 9l6 6 6-6"/></svg></summary>
        <div class="menu-list">
          <div class="menu-row"><span class="name">Coca-Cola 350ml</span><span class="leader"></span><span class="price">R$ 7,00</span></div>
          <div class="menu-row"><span class="name">Fanta Laranja 350ml</span><span class="leader"></span><span class="price">R$ 7,00</span></div>
          <div class="menu-row"><span class="name">Sprite 350ml</span><span class="leader"></span><span class="price">R$ 7,00</span></div>
          <div class="menu-row"><span class="name">Coca-Cola Zero 350ml</span><span class="leader"></span><span class="price">R$ 7,00</span></div>
          <div class="menu-row"><span class="name">Água Mineral 500ml</span><span class="leader"></span><span class="price">R$ 4,00</span></div>
          <div class="menu-row"><span class="name">Água com Gás 500ml</span><span class="leader"></span><span class="price">R$ 4,00</span></div>
        </div>
      </details>

      <details>
        <summary>Tortas <span class="count">2 itens</span> <svg class="icon chev" viewBox="0 0 24 24"><path d="M6 9l6 6 6-6"/></svg></summary>
        <div class="menu-list">
          <div class="menu-row"><span class="name">Torta de frango c/ Catupiry (500g) <span class="tag tag-new">Novidade</span></span><span class="leader"></span><span class="price">R$ 20,00</span></div>
          <div class="menu-row"><span class="name">Torta de carne seca c/ Catupiry (500g)</span><span class="leader"></span><span class="price">R$ 24,00</span></div>
        </div>
      </details>

      <details>
        <summary>Milho Cozido <span class="count">1 item</span> <svg class="icon chev" viewBox="0 0 24 24"><path d="M6 9l6 6 6-6"/></svg></summary>
        <div class="menu-list">
          <div class="menu-row"><span class="name">Milho cozido no potinho</span><span class="leader"></span><span class="price">A partir de R$ 12,00</span></div>
        </div>
      </details>

      <details>
        <summary>Caldo <span class="count">1 item</span> <svg class="icon chev" viewBox="0 0 24 24"><path d="M6 9l6 6 6-6"/></svg></summary>
        <div class="menu-list">
          <div class="menu-row"><span class="name">Caldo de milho (500g)</span><span class="leader"></span><span class="price">R$ 25,00</span></div>
        </div>
      </details>

      <details>
        <summary>Coxinha de Milho <span class="count">1 item</span> <svg class="icon chev" viewBox="0 0 24 24"><path d="M6 9l6 6 6-6"/></svg></summary>
        <div class="menu-list">
          <div class="menu-row"><span class="name">Porção de coxinha (15 mini) <span class="tag tag-new">Novidade</span></span><span class="leader"></span><span class="price">R$ 19,90</span></div>
        </div>
      </details>
    </div>
  </div>
</section>

<!-- FINAL CTA -->
<section class="section">
  <div class="wrap">
    <div class="final-cta">
      <h2>Sua pamonha tá a um clique de distância</h2>
      <p>Pedido mínimo de R$ 15,00, feito na hora e entregue quentinho em Jardim D'Icaraí e região.</p>
      <a class="btn" href="https://pedido.brendi.com.br/emporio-da-pamonha-jardim-dicarai/" target="_blank" rel="noopener">Fazer meu pedido agora →</a>
      <small>Pedido, pagamento e acompanhamento acontecem direto na plataforma Brendi.</small>
    </div>
  </div>
</section>

<footer>
  <div class="wrap footer-inner">
    <div>🌽 Empório da Pamonha — Jardim D'Icaraí, Salto - SP</div>
    <div>Cardápio e pedidos via Brendi · CNPJ 37.593.578/0001-09</div>
  </div>
</footer>

<div class="sticky-bar">
  <p>Pedido mínimo<strong>R$ 15,00</strong></p>
  <a class="btn btn-sm" href="https://pedido.brendi.com.br/emporio-da-pamonha-jardim-dicarai/" target="_blank" rel="noopener">Fazer pedido →</a>
</div>

</body>
</html>
