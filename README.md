# elisa.clerc
<!DOCTYPE html>
<html lang="fr">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>Elisa Clerc – Étudiante en publicité</title>
<meta name="description" content="Elisa Clerc, étudiante en BUT Info-Com parcours publicité à l'IUT Bordeaux Montaigne. À la recherche d'un stage en agence.">
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Archivo:wdth,wght@62..125,100..900&display=swap" rel="stylesheet">
<style>
:root{
  --black:#000; --soft:#111; --white:#fff; --orange:#ff6a00; --line:rgba(255,255,255,.22);
  --pad:clamp(20px,5vw,72px);
}
*{box-sizing:border-box;margin:0}
html{scroll-behavior:smooth;scroll-padding-top:60px}
body{font-family:'Archivo',Arial,sans-serif;background:var(--black);color:var(--white);line-height:1.55;font-size:18px}
a{color:inherit}
:focus-visible{outline:3px solid var(--orange);outline-offset:3px}

/* Barre de progression du scroll */
#progress{position:fixed;top:0;left:0;height:4px;width:0;background:var(--orange);z-index:30}

/* Bannière */
header{position:fixed;top:0;left:0;right:0;z-index:20;display:flex;justify-content:space-between;align-items:center;padding:0 var(--pad);height:60px;background:var(--black);color:var(--white);border-bottom:1px solid var(--line)}
header .logo{color:var(--orange);font-weight:900;font-size:1.2rem;text-decoration:none;letter-spacing:-.02em}
nav{display:flex;gap:clamp(14px,3vw,36px)}
nav a{text-decoration:none;font-weight:600;font-size:.95rem}
nav a:hover{color:var(--orange);text-decoration:underline;text-underline-offset:6px}

/* Vidéo plein écran sous la bannière */
.reel{margin-top:60px;height:calc(100vh - 60px);height:calc(100svh - 60px);background:var(--black);position:relative}
.slot{position:absolute;inset:0;display:grid;place-items:center}
.slot::before{content:"";width:0;height:0;border-style:solid;border-width:28px 0 28px 46px;border-color:transparent transparent transparent var(--orange);opacity:.9}
.slot video{position:absolute;inset:0;width:100%;height:100%;object-fit:cover;background:#000}
.slot video:not([Create an 8-second photorealisti 2837 Z7i])~*{display:none}

section{padding:clamp(64px,10vw,130px) var(--pad)}
h2{color:var(--orange);font-weight:900;font-stretch:80%;font-size:clamp(2.2rem,6vw,4.8rem);line-height:.95;letter-spacing:-.025em;margin-bottom:40px;max-width:16ch}

/* Présentation */
.intro{display:grid;grid-template-columns:1fr 1fr;gap:clamp(24px,6vw,90px)}
.intro p{max-width:52ch;margin-bottom:1em}
.intro .big{font-size:clamp(1.3rem,2.4vw,1.9rem);font-weight:600;line-height:1.3}
.skills{border-top:2px solid var(--orange);margin-top:56px;padding:0}
.skills li{list-style:none;display:grid;grid-template-columns:minmax(120px,1fr) 2fr;gap:24px;padding:22px 0;border-bottom:1px solid var(--line)}
.skills strong{color:var(--orange);font-size:1.35rem;font-weight:800}

/* Projets */
#projets{background:var(--soft)}
.proj{display:grid;grid-template-columns:1.1fr 1fr;gap:clamp(20px,5vw,70px);padding:36px 0;border-top:1px solid var(--line);align-items:center}
.proj .img{aspect-ratio:4/3;background:#000;border:2px solid var(--orange);color:var(--orange);border-radius:6px;display:grid;place-items:center;font-weight:800;font-size:1.1rem;overflow:hidden}
.proj .img img{width:100%;height:100%;object-fit:cover}
.proj h3{color:var(--orange);font-size:clamp(1.6rem,3vw,2.4rem);font-weight:900;font-stretch:85%;line-height:1.05;margin-bottom:12px}
.proj p{max-width:46ch;opacity:.85}
.tags{margin-top:16px;display:flex;flex-wrap:wrap;gap:8px}
.tags span{border:1px solid var(--orange);color:var(--orange);border-radius:999px;padding:3px 14px;font-size:.9rem}

/* Contact */
#contact{background:#000;border-top:1px solid var(--line)}
#contact h2{max-width:20ch}
.contact-list{display:grid;gap:10px;font-size:clamp(1.2rem,2.5vw,1.8rem);font-weight:700}
.contact-list a:hover{color:var(--orange)}
.contact-list a{text-underline-offset:6px}
footer{background:#000;border-top:1px solid var(--line);color:var(--white);padding:24px var(--pad);font-size:.9rem}

@media(max-width:760px){
  .intro,.proj,.skills li{grid-template-columns:1fr}
  .skills li{gap:4px}
  nav a{font-size:.85rem}
}
@media(prefers-reduced-motion:reduce){html{scroll-behavior:auto}}
</style>
</head>
<body>
<div id="progress" aria-hidden="true"></div>

<header>
  <a class="logo" href="#accueil">Elisa Clerc</a>
  <nav aria-label="Navigation principale">
    <a href="#accueil">Accueil</a>
    <a href="#presentation">Présentation</a>
    <a href="#projets">Projets</a>
    <a href="#contact">Me contacter</a>
  </nav>
</header>

<main>
  <!-- ACCUEIL : vidéo plein écran sous la bannière -->
  <div class="reel" id="accueil">
    <div class="slot">
      <!-- Pour activer la vidéo : mets ton fichier dans le dossier assets/ puis écris src="assets/ma-video.mp4" -->
      <video controls playsinline preload="metadata" src="" hidden></video>
    </div>
  </div>

  <!-- PRÉSENTATION -->
  <section id="presentation">
    <h2>Qui je suis</h2>
    <div class="intro">
      <p class="big">Je suis en 2e année de BUT Information-Communication, parcours publicité, à l'IUT Bordeaux Montaigne.</p>
      <div>
        <p>J'aime construire des idées qui se vivent sur le terrain : une stratégie claire, un événement, un contenu qui donne envie.</p>
        <p>SPK accompagne les acteurs du sport avec ses trois piliers, Produit, Pratique et Passion. C'est l'univers dans lequel je veux apprendre le métier.</p>
      </div>
    </div>
    <ul class="skills">
      <!-- Modifie ces lignes avec tes vraies compétences -->
      <li><strong>Stratégie</strong><span>Analyse d'une marque, de sa cible et de ses concurrents, puis recommandation.</span></li>
      <li><strong>Événementiel</strong><span>Imaginer un dispositif sur plusieurs villes avec un budget donné.</span></li>
      <li><strong>Contenus et social</strong><span>Rédaction, idées de formats et animation de communautés.</span></li>
      <li><strong>Création</strong><span>Outils graphiques et veille culturelle.</span></li>
    </ul>
  </section>

  <!-- PROJETS -->
  <section id="projets">
    <h2>Mes projets</h2>

    <article class="proj">
      <div class="img"><!-- <img src="assets/nike.jpg" alt="Projet Nike"> -->Visuel du projet</div>
      <div>
        <h3>Nike : la course pour les débutants</h3>
        <p>Brief d'annonceur : un événement de course à pied pour débutants dans trois villes universitaires françaises, avec un budget de 50 000 €.</p>
        <div class="tags"><span>Stratégie</span><span>Événementiel</span></div>
      </div>
    </article>

    <article class="proj">
      <div class="img"><!-- <img src="assets/newwork.jpg" alt="Agence New Work"> -->Visuel du projet</div>
      <div>
        <h3>New Work, une agence new-yorkaise</h3>
        <p>Création d'une agence fictive : nom, personnalité, promesse, code visuel, logo et règle d'agence.</p>
        <div class="tags"><span>Identité de marque</span><span>Création</span></div>
      </div>
    </article>

    <article class="proj">
      <div class="img"><!-- <img src="assets/respire.jpg" alt="Enquête Respire"> -->Visuel du projet</div>
      <div>
        <h3>Respire, enquête de marque</h3>
        <p>Travail de groupe sur une marque de beauté : analyse de sa présence payée, gagnée et possédée, de sa cible et des avis.</p>
        <div class="tags"><span>Analyse</span><span>Social</span></div>
      </div>
    </article>
  </section>

  <!-- CONTACT -->
  <section id="contact">
    <h2>Travaillons ensemble</h2>
    <div class="contact-list">
      <!-- Remplace par tes vraies coordonnées -->
      <a href="mailto:ton.email@exemple.fr">ton.email@exemple.fr</a>
      <a href="tel:+33000000000">06 00 00 00 00</a>
      <a href="https://www.linkedin.com/in/ton-profil">LinkedIn</a>
      <a href="assets/CV.pdf">Mon CV (PDF)</a>
    </div>
  </section>
</main>

<footer>Fait par Elisa Clerc, BUT Info-Com publicité, IUT Bordeaux Montaigne</footer>

<script>
const bar=document.getElementById('progress');
function update(){
  const h=document.documentElement;
  const max=h.scrollHeight-h.clientHeight;
  bar.style.width=(max>0?h.scrollTop/max*100:0)+'%';
}
addEventListener('scroll',update,{passive:true});
update();
// Affiche la vidéo dès qu'un fichier est renseigné
const v=document.querySelector('.slot video');
if(v&&v.getAttribute('src')){v.hidden=false;}
</script>
</body>
</html>
