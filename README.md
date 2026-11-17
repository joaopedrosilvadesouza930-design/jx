[index.html](https://github.com/user-attachments/files/34970590/index.html)
<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1, viewport-fit=cover">
<title>RF1 Mods Brasil</title>
<style>
:root{--bg:#f3f4f6;--card:#fff;--tx:#14171c;--mu:#667085;--ac:#e5322d;--bd:#e2e5ea;--hd:#101319;--dc:#5865f2;box-sizing:border-box;padding-top:env(safe-area-inset-top,0px);padding-bottom:env(safe-area-inset-bottom,0px)}
@media (prefers-color-scheme:dark){:root:not([data-theme="light"]){--bg:#0d0f13;--card:#171a20;--tx:#eef0f3;--mu:#98a2b3;--bd:#262b33}}
:root[data-theme="dark"]{--bg:#0d0f13;--card:#171a20;--tx:#eef0f3;--mu:#98a2b3;--bd:#262b33}
html{scroll-padding-top:calc(env(safe-area-inset-top,0px) + 60px)}
*{box-sizing:border-box}
body{margin:0;background:var(--bg);color:var(--tx);font-family:system-ui,-apple-system,"Segoe UI",Roboto,sans-serif;line-height:1.5}
body::before{content:"";position:fixed;inset:0 0 auto;height:env(safe-area-inset-top,0px);background:var(--hd);z-index:10}
header{position:sticky;top:env(safe-area-inset-top,0px);background:var(--hd);z-index:9;border-bottom:3px solid var(--ac)}
.w{max-width:1100px;margin:0 auto;padding:0 14px}
.nav{display:flex;align-items:center;gap:14px;height:54px;overflow-x:auto;white-space:nowrap}
.logo{font-weight:800;font-size:1.2rem;color:#fff;text-decoration:none;letter-spacing:.5px}.logo b{color:var(--ac)}
.nav a{color:#c9ced6;text-decoration:none;font-size:.92rem}
.nav .sp{flex:1}
.btn{display:inline-block;background:var(--ac);color:#fff;border:0;text-decoration:none;padding:8px 14px;border-radius:8px;font-weight:600;cursor:pointer;font-size:.9rem}
.btn.d{background:var(--dc)}
.hero{background:linear-gradient(135deg,#1b1f27,#2b0f10);color:#fff;padding:30px 0 26px}
.hero h1{margin:0 0 6px;font-size:1.7rem}.hero p{margin:0 0 14px;color:#c9ced6}
.hero input{width:100%;padding:13px 14px;border-radius:10px;border:0;font-size:1rem;background:#fff;color:#14171c}
.tabs{display:flex;gap:6px;overflow-x:auto;padding:14px 0 6px}
.tab{border:1px solid var(--bd);background:var(--card);color:var(--tx);padding:8px 14px;border-radius:99px;cursor:pointer;white-space:nowrap;font-size:.9rem}
.tab.on{background:var(--ac);border-color:var(--ac);color:#fff}
.row{display:flex;justify-content:space-between;align-items:center;margin:8px 0}
select{padding:7px 10px;border-radius:8px;border:1px solid var(--bd);background:var(--card);color:var(--tx)}
h2{font-size:1.15rem;margin:22px 0 8px;border-left:4px solid var(--ac);padding-left:8px}
.g{display:grid;grid-template-columns:repeat(auto-fill,minmax(250px,1fr));gap:12px}
.c{background:var(--card);border:1px solid var(--bd);border-radius:12px;overflow:hidden;cursor:pointer}
.th{height:120px;display:flex;align-items:flex-end;padding:8px;color:#fff;font-weight:700;font-size:1.6rem}
.cb{padding:12px}.cb h3{margin:0 0 2px;font-size:1rem}.cb p{margin:4px 0 8px;color:var(--mu);font-size:.88rem}
.m{display:flex;justify-content:space-between;color:var(--mu);font-size:.82rem}
.tg{display:inline-block;font-size:.72rem;background:var(--ac);color:#fff;padding:1px 8px;border-radius:5px}
.news{display:grid;grid-template-columns:repeat(auto-fill,minmax(250px,1fr));gap:12px}
.n{background:var(--card);border:1px solid var(--bd);border-radius:12px;padding:14px}.n small{color:var(--mu)}.n h3{margin:4px 0;font-size:1rem}
.dc{background:var(--card);border:1px solid var(--bd);border-radius:12px;padding:18px;margin:24px 0}
.md{position:fixed;inset:0;background:rgba(0,0,0,.6);display:none;align-items:center;justify-content:center;padding:16px;z-index:20}
.md.on{display:flex}.mb{background:var(--card);border-radius:14px;max-width:460px;width:100%;overflow:hidden;max-height:90%;overflow-y:auto}
.mb .th{height:150px}.mb .cb{padding:16px}
footer{color:var(--mu);font-size:.85rem;padding:10px 0 30px}
</style>
</head>
<body>
<header><div class="w nav">
<a class="logo" href="#">RF1<b>MODS</b></a>
<a href="#mods">Mods</a><a href="#noticias">Notícias</a><a href="#discord">Discord</a>
<span class="sp"></span>
<a class="btn" href="#discord">Enviar mod</a>
</div></header>
<section class="hero"><div class="w">
<h1>Mods para rFactor 1</h1>
<p>Carros, pistas, skins e plugins da comunidade brasileira.</p>
<input id="q" placeholder="Buscar carros, pistas, plugins..." aria-label="Buscar">
</div></section>
<div class="w">
<div class="tabs" id="tabs"></div>
<div class="row"><span id="cnt" style="color:var(--mu);font-size:.9rem"></span>
<select id="ord" aria-label="Ordenar"><option value="r">Mais recentes</option><option value="d">Mais baixados</option><option value="n">Melhor nota</option></select></div>
<h2 id="mods">Mods</h2>
<div class="g" id="g"></div>
<h2 id="noticias">Notícias</h2>
<div class="news">
<div class="n"><small>Dica</small><h3>Como instalar um mod no rFactor 1</h3><p>Extraia na pasta GameData ou use o instalador .rfm.</p></div>
<div class="n"><small>Guia</small><h3>Otimize carros para PCs fracos</h3><p>Reduza texturas, LODs e RAM sem perder qualidade.</p></div>
<div class="n"><small>Comunidade</small><h3>Corridas online toda semana</h3><p>Veja horários e servidores no nosso Discord.</p></div>
</div>
<section class="dc" id="discord">
<h2 style="margin-top:0">Comunidade no Discord</h2>
<p style="color:var(--mu)">Tire dúvidas, envie seus mods e entre nas corridas online.</p>
<a class="btn d" id="dl" href="#discord">Entrar no servidor</a>
</section>
<footer>Mods pertencem aos seus autores. Envie apenas conteúdo com permissão de distribuição.</footer>
</div>
<div class="md" id="md"><div class="mb" id="mb"></div></div>
<script>
var DISCORD="https://discord.gg/SEU-CONVITE";
var MODS=[
{n:"Oreca 07 otimizado",t:"Carros",a:"Autor1",d:"LMP2 com LODs e texturas leves para PCs modestos.",v:"1.0",dl:1240,r:4.8,o:5,c:"#c0392b"},
{n:"Circuito exemplo",t:"Pistas",a:"Autor2",d:"Pista de demonstração com GMT otimizado.",v:"1.2",dl:860,r:4.5,o:4,c:"#1e8449"},
{n:"Plugin de chat fixo",t:"Plugins",a:"Autor3",d:"Mostra o chat permanentemente na tela.",v:"0.1",dl:410,r:4.6,o:3,c:"#2e86c1"},
{n:"Radar de proximidade",t:"Plugins",a:"Autor3",d:"Radar de carros próximos para o rFactor 1.",v:"0.1",dl:520,r:4.4,o:2,c:"#8e44ad"},
{n:"Pack de skins online",t:"Skins",a:"Autor4",d:"Skins para as corridas da comunidade.",v:"1.0",dl:300,r:4.2,o:1,c:"#d68910"},
{n:"Sons realistas V8",t:"Sons",a:"Autor5",d:"Pacote de áudio para motores V8.",v:"2.1",dl:700,r:4.7,o:6,c:"#566573"}
];
var cats=["Todos","Carros","Pistas","Skins","Plugins","Sons"],tipo="Todos";
function esc(s){return String(s).replace(/[&<>"]/g,function(c){return{"&":"&amp;","<":"&lt;",">":"&gt;",'"':"&quot;"}[c]})}
function th(m,cl){return '<div class="'+cl+'" style="background:linear-gradient(135deg,'+m.c+',#111)">'+esc(m.n.charAt(0))+'</div>'}
function draw(){
var q=document.getElementById("q").value.toLowerCase(),o=document.getElementById("ord").value;
document.getElementById("tabs").innerHTML=cats.map(function(c){return '<button class="tab'+(c==tipo?' on':'')+'" data-c="'+c+'">'+c+'</button>'}).join("");
var l=MODS.map(function(m,i){m.i=i;return m}).filter(function(m){return(tipo=="Todos"||m.t==tipo)&&(m.n+m.d+m.a).toLowerCase().indexOf(q)>-1});
l.sort(function(a,b){return o=="d"?b.dl-a.dl:o=="n"?b.r-a.r:a.o-b.o});
document.getElementById("cnt").textContent=l.length+" mods";
document.getElementById("g").innerHTML=l.map(function(m){return '<div class="c" data-i="'+m.i+'">'+th(m,"th")+'<div class="cb"><span class="tg">'+esc(m.t)+'</span><h3>'+esc(m.n)+'</h3><p>'+esc(m.d)+'</p><div class="m"><span>por '+esc(m.a)+'</span><span>⬇ '+m.dl+' · ★ '+m.r+'</span></div></div></div>'}).join("");
}
document.getElementById("tabs").addEventListener("click",function(e){if(e.target.dataset.c){tipo=e.target.dataset.c;draw()}});
document.getElementById("q").addEventListener("input",draw);
document.getElementById("ord").addEventListener("change",draw);
document.getElementById("g").addEventListener("click",function(e){var c=e.target.closest(".c");if(!c)return;var m=MODS[c.dataset.i];
document.getElementById("mb").innerHTML=th(m,"th")+'<div class="cb"><span class="tg">'+esc(m.t)+'</span><h3>'+esc(m.n)+'</h3><p>'+esc(m.d)+'</p><p>Autor: '+esc(m.a)+' · v'+esc(m.v)+' · ⬇ '+m.dl+' · ★ '+m.r+'</p><a class="btn" href="'+DISCORD+'">Baixar no Discord</a> <button class="btn d" id="x">Fechar</button></div>';
document.getElementById("md").classList.add("on");document.getElementById("x").onclick=function(){document.getElementById("md").classList.remove("on")}});
document.getElementById("md").addEventListener("click",function(e){if(e.target.id=="md")this.classList.remove("on")});
document.getElementById("dl").href=DISCORD;
draw();
</script>
</body>
</html>
