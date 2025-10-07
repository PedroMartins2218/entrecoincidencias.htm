<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Coincidências — ou talvez só boas histórias que se repetem</title>
  <meta name="description" content="Um quiz leve pra descobrir combinações improváveis — daquelas que às vezes acontecem fora da tela também.">
  <style>
    :root{
      --bg:#f8fafc;
      --sand:#fff7ed;
      --sea:#c7d2fe;
      --ink:#0f172a;
      --muted:#475569;
      --accent:#60a5fa;
      --accent-2:#34d399;
      --ring:rgba(96,165,250,.35);
      --card:#ffffff;
      --radius:18px;
      --shadow:0 10px 28px rgba(2,6,23,.08);
    }
    *{box-sizing:border-box}
    html,body{height:100%}
    body{
      margin:0;
      font-family: ui-sans-serif, -apple-system, Segoe UI, Roboto, Helvetica, Arial;
      color:var(--ink);
      background:linear-gradient(180deg, var(--bg), #eef2ff 50%, #e0e7ff 60%, #dbeafe 70%, #e2e8f0 100%);
      display:grid; place-items:center;
      overflow-x:hidden;
    }
    main{
      width:min(800px, 92vw);
      background:var(--card);
      border-radius:var(--radius);
      box-shadow:var(--shadow);
      border:1px solid #eef2ff;
      padding:clamp(18px, 3vw, 28px);
      z-index:1; position:relative;
    }
    .badge{
      background: linear-gradient(135deg, var(--accent), var(--accent-2));
      color:#fff; padding:8px 12px; border-radius:999px;
      font-size:12px; letter-spacing:.3px; box-shadow:0 8px 18px var(--ring);
    }
    h1{font-size:clamp(22px, 4.5vw, 32px); margin:6px 0;}
    p.lead{color:var(--muted); margin:0 0 16px;}
    .card{background:linear-gradient(180deg, #ffffff, var(--sand)); border:1px solid #f1f5f9;
      border-radius:14px; padding:14px; margin:12px 0; box-shadow:0 6px 18px rgba(2,6,23,.04);}
    .opts{display:grid; gap:8px;} @media(min-width:560px){.opts{grid-template-columns:repeat(2,1fr);}}
    button.opt{background:#fff; border:1px solid #e2e8f0; border-radius:12px; padding:12px 14px; cursor:pointer;
      transition:all .2s; text-align:left;}
    button.opt:hover{border-color:#cbd5e1; box-shadow:0 8px 16px rgba(2,6,23,.08);}
    button.opt[aria-pressed="true"]{border-color:#93c5fd; box-shadow:0 10px 22px rgba(147,197,253,.35); background:linear-gradient(180deg,#fff,#f0f9ff);}
    .actions{display:flex; justify-content:flex-end; gap:10px; margin-top:12px;}
    .btn{background:linear-gradient(135deg, var(--accent), var(--accent-2)); color:#fff; padding:12px 14px; border:none; border-radius:12px; cursor:pointer;}
    .ghost{background:#fff; color:var(--ink); border:1px solid #e2e8f0;}
    footer{display:flex; justify-content:space-between; font-size:12px; color:var(--muted); margin-top:10px;}
  </style>
</head>
<body>
  <main>
    <span class="badge">Coincidências</span>
    <h1>Coincidências — ou talvez só boas histórias que se repetem.</h1>
    <p class="lead">Um quiz leve (e sem pressa) pra descobrir combinações improváveis — daquelas que às vezes acontecem fora da tela também.</p>

    <section class="card" data-q="1">
      <h3>Um sábado perfeito tem mais cara de...</h3>
      <div class="opts">
        <button class="opt" data-val="Café + livro">☕ Café + livro</button>
        <button class="opt" data-val="Praia + sol">🌴 Praia + sol</button>
        <button class="opt" data-val="Filme + cobertor">🎥 Filme + cobertor</button>
        <button class="opt" data-val="Treino + descanso">🥋 Treino + descanso</button>
      </div>
    </section>

    <section class="card" data-q="2">
      <h3>Se a sua história fosse um romance, estaria mais perto de...</h3>
      <div class="opts">
        <button class="opt" data-val="Cartas para Julieta">💌 Cartas para Julieta</button>
        <button class="opt" data-val="Questão de Tempo">⏳ Questão de Tempo</button>
        <button class="opt" data-val="Enrolados (Rapunzel)">🪞 Enrolados (Rapunzel)</button>
        <button class="opt" data-val="Para Todos os Garotos que Já Amei">💗 Para Todos os Garotos que Já Amei</button>
      </div>
    </section>

    <section class="card" data-q="3">
      <h3>Seu elemento favorito pra recarregar as energias é...</h3>
      <div class="opts">
        <button class="opt" data-val="Água (natação, mar)">💧 Água (natação, mar)</button>
        <button class="opt" data-val="Praia (areia e brisa)">🌴 Praia (areia e brisa)</button>
        <button class="opt" data-val="Ar (vista alta, vento leve)">🌬️ Ar (vista alta, vento leve)</button>
        <button class="opt" data-val="Fogo (ritmo de treino)">🔥 Fogo (ritmo de treino)</button>
      </div>
    </section>

    <section class="card" data-q="4">
      <h3>No tatame, você é mais...</h3>
      <div class="opts">
        <button class="opt" data-val="Técnica paciente">🧩 Técnica paciente</button>
        <button class="opt" data-val="Explosão com controle">⚡ Explosão com controle</button>
        <button class="opt" data-val="Estratégia silenciosa">🧠 Estratégia silenciosa</button>
        <button class="opt" data-val="Movimento fluido">🌊 Movimento fluido</button>
      </div>
    </section>

    <section class="card" data-q="5">
      <h3>Animais que te ganham no primeiro olhar...</h3>
      <div class="opts">
        <button class="opt" data-val="Cachorros">🐶 Cachorros</button>
        <button class="opt" data-val="Gatos">🐱 Gatos</button>
        <button class="opt" data-val="Golfinhos / Tartarugas">🐬 Golfinhos / 🐢 Tartarugas</button>
        <button class="opt" data-val="Passarinhos">🐦 Passarinhos</button>
      </div>
    </section>

    <section class="card">
      <p>Engraçado como certas coincidências acabam acontecendo no mesmo lugar.<br>
      Desde aquele domingo no PP, fiquei com a sensação de que algumas histórias ficam ecoando na cabeça..</p>
    </section>

    <div class="actions">
      <button class="btn ghost" id="random">Surpreenda-me</button>
      <button class="btn" id="see">Ver resultado</button>
    </div>

    <section class="card" id="result" hidden>
      <h3>Seu resultado:</h3>
      <div id="pillbox" style="display:flex;flex-wrap:wrap;gap:8px;"></div>
      <p id="text" style="margin-top:10px;color:#475569;"></p>
      <div class="actions">
        <a class="btn ghost" id="reset" href="#">Refazer</a>
        <a class="btn" id="share" href="#">continuar o papo</a>
      </div>
    </section>

    <footer><span>Sem cadastro, só curiosidade.</span><span>Feito com HTML + CSS + boas coincidências.</span></footer>
  </main>

  <script>
    const choices={},cards=document.querySelectorAll('[data-q]');
    cards.forEach(c=>c.querySelectorAll('.opt').forEach(b=>b.onclick=()=>{
      c.querySelectorAll('.opt').forEach(o=>o.setAttribute('aria-pressed','false'));
      b.setAttribute('aria-pressed','true'); choices[c.dataset.q]=b.dataset.val;
    }));
    document.getElementById('random').onclick=()=>cards.forEach(c=>{
      const o=[...c.querySelectorAll('.opt')]; o[Math.floor(Math.random()*o.length)].click();
    });
    const res=document.getElementById('result'),pill=document.getElementById('pillbox'),txt=document.getElementById('text');
    document.getElementById('see').onclick=()=>{
      if(Object.keys(choices).length===cards.length){
        pill.innerHTML=''; Object.values(choices).forEach(v=>{
          const s=document.createElement('span'); s.textContent=v; s.style.padding='8px 10px'; s.style.border='1px solid #cbd5e1'; s.style.borderRadius='999px';
          pill.appendChild(s);
        });
        txt.textContent=`Parece que seus gostos seguem uma linha leve — meio ${choices['1'].toLowerCase()}, ${choices['2'].toLowerCase()} e ${choices['3'].toLowerCase()}. Coincidências assim merecem ser testadas fora da tela, né?`;
        res.hidden=false; res.scrollIntoView({behavior:'smooth'});
      }else alert('Escolha uma opção em cada cartão :)');
    };
    document.getElementById('reset').onclick=e=>{e.preventDefault();for(const k in choices)delete choices[k];
      cards.forEach(c=>c.querySelectorAll('.opt').forEach(b=>b.setAttribute('aria-pressed','false')));res.hidden=true;window.scrollTo({top:0,behavior:'smooth'});};
    document.getElementById('share').onclick=e=>{e.preventDefault();
      const msg=encodeURIComponent('Parece que a coincidência do Panorama ainda tá rendendo assunto 😅\\nBora ver se ela se repete?');
      window.open('https://wa.me/?text='+msg,'_blank','noopener');
    };
  </script>
</body>
</html>
