<head>
    <meta name="author" content="Riona Kelly">
</head>

<script>
    import { base } from '$app/paths';
    import { onMount } from 'svelte';
  
    onMount(() => {
      console.log("Portfolio Page Loaded");
    })
</script>

<div>
  <h1>Portfolio</h1>
  <p class="intro">Here are the past projects that I have worked on either in college, events, or in my own time. 
  <br>I'll be updating this whenever I have a new projects that I want to show off so that you can all ready more about it and hopefully try it out!</p>
  <h2>Games</h2>
</div>
<div class="grid">
  <a href="{base}/portfolio/games/desktoppet">
  <div>
    <img src="{base}/DesktopPetSS.png" alt="Screenshot of pixelated animals on a computer desktop">
    <h2>My Desktop Pet</h2>
    <p>This is a simple virtual pet that will live on your desktop and you can raise and take care of while using your computer. 
      I am currently working on this full time at it is my project for this college semester. 
      While it is still a work in progress you can download beta versions here and to try it out!</p>
    <!--<img src="{base}/itchio.png" alt="clickable itch logo" class="icon">-->
  </div>
  </a>

  <a href="https://shadowmalteser.itch.io/fishybusiness" target="_blank"><!--<a href="{base}/portfolio/games/fishybusiness">-->
  <div>
    <img src="{base}/FishyBusinessCover.png" alt="Green monster in detective outfit with chip shop owner and the title 'An Phiast in: Fishy Business'">
    <h2>An Phiast in: Fishy Business</h2>
    <p>This is my team's Game Sting submisson for the <u>2026 Dingle Animation Festival</u>!
      A short comedic detective game where An Phiast must try to solve the mystery of who stole 'The Perfect Fish and Chips'. 
      I worked on design with my team, dialogue, menus, and modelling an area.</p>
  </div>
  </a>

  <a href="https://shadowmalteser.itch.io/starburst" target="_blank"><!--<a href="{base}/portfolio/games/starburst">  -->
  <div>
    <img src="{base}/StarburstSS.png" alt="Screenshot of a spaceship and planet with the title 'Starburst'">
    <h2>Starburst</h2>
    <p>My friend and I's entry to the <u>2025 Games Fleadh</u>, Starburst, is a fast paced 2D Shooter where you grab asteroids flying past you you and throw them towards planets to destroy them and harvest their cores. 
      We were awarded <u><i>Best Game using Libraries</i></u> and <u><i>Best Game Mechanics</i></u> at the event.</p>
  </div>
  </a>

  <a href="https://michael-r-ryan.itch.io/unmasked" target="_blank"><!--<a href="{base}/portfolio/games/unmasked">-->
  <div>
    <img src="{base}/UnmaskedSS.png" alt="Pixel art of village with the title 'Unmasked'">
    <h2>Unmasked</h2>
    <p>A short narrative game that I made with my team for the <u>2026 Global Game Jam</u> about helping village people who have been cursed by a witch to wear masks that represent their fears and insecurities. 
      Play as a wizard therapist and explore the psyches of the townspeople, and break the curse.</p>
  </div>
  </a>

  <a href="{base}/portfolio/notyet">
  <div>
    <img src="{base}/GoldDivers.jpg" alt="3 people playing handmade board game with cardboard tiles and divers">
    <h2>Gold Divers</h2>
    <p>A board game that I made with my team for the <u>2025 Global Game Jam</u> with my college. You must explore the depths by placing random tiles to try and find treasure to bring back up to the surface.</p>
  </div>
  </a>

  <a href="{base}/portfolio/notyet">
  <div>
    <img src="{base}/PaintPartySS.png" alt="Screenshot of pixel-art characters painting a floor in a game">
    <h2>Paint Party</h2>
    <p>Paint Party is a multiplayer party game using SFML I made in college with a group, where the players must cover as much area as they can in paint to win. I coded all of the gameplay while my teammates made the assets and menus.</p>
  </div>
  </a>
</div>

<div>
  <h2>Websites</h2>
</div>
<div class="grid">
<div></div>
  <a href="{base}/portfolio/notyet">
  <div>
    <img src="{base}/WebsiteThumbnail.png" alt="Screenshot of pixel-art characters painting a floor in a game">
    <h2>My Portfolio</h2>
    <p>The website you're looking at right now! I made this in March to showcase all of my work and let people learn more about me. 
      I'm really proud of it so far and I plan to keep working on it to make it more "me" whenever I can. :D</p>
  </div>
  </a>
</div>


<style>
h1 {
  grid-area: title;
  padding: 16px;
  font-weight: bold;
  font-size: 48px;
  text-align: center;
}

h2 {
  font-weight: bold;
  font-size: 32px;
  text-align: center;
}

p {
  font-size: 20px;
}

.intro {
  padding-left: 50px;
  font-size: 22px;
}

.grid {
  display: grid;
  grid-template-columns: repeat(3, minmax(0, 1fr));
  padding: 32px;
  padding-top: 0px;

}

.grid h2 {
  font-weight: bold;
  font-size: 24px;
  color: var(--primary-color);
  text-align: left;
}

.grid div {
  padding: 12px;
  padding-left: 16px;
  padding-right: 16px;
}

.grid img {
  max-width: 100%;
  max-height: 100%;
  border-radius: 12px;
}

a {
    color: var(--text-color);
    text-decoration: none;
}

a:hover {
    filter: saturate(120%);
    h2 {
      text-decoration: underline;
    }
}

/*
.c1 {
  float: left;
  width: 33%;
  padding: 16px;
}
.c2 {
  float: left;
  width: 33%;
  padding: 16px;
}
.c3 {
  float: right;
  width: 33%;
  padding: 16px;
}
.c1 p {
  padding-left: 0;
}
.c2 p {
  padding-left: 0;
}
.c3 p {
  padding-left: 0;
}*/

/* Mobile Navigation:*/
@media (max-width: 1200px) {
  .grid {
    display:block;
    grid-template-columns: auto;
  }

  .grid img {
  display: block;
  margin-left: auto;
  margin-right: auto;
  width: 100%;
  margin-bottom: 16px;
  }
}
</style>
