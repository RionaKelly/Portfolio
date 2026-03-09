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
</div>
<div class="grid">
  <a href="{base}/portfolio/games/desktoppet">
  <div>
    <img src="{base}/DesktopPetSS.png" alt="Screenshot of a game with a spaceship and planet in space">
    <h2>My Desktop Pet</h2>
    <p>My team's entry to the 2025 Games Fleadh, Starburst, is a fast paced 2D Shooter where you grab asteroids around you and throw them at planets to destroy them and harvest their cores.</p>
  </div>
  </a>
  <a href="https://shadowmalteser.itch.io/fishybusiness" target="_blank"><!--<a href="{base}/portfolio/games/fishybusiness">-->
  <div>
    <img src="{base}/FishyBusinessCover.png" alt="Screenshot of a game with a spaceship and planet in space">
    <h2>An Phiast in: Fishy Business</h2>
    <p>My team's entry to the 2025 Games Fleadh, Starburst, is a fast paced 2D Shooter where you grab asteroids around you and throw them at planets to destroy them and harvest their cores.</p>
  </div>
  </a>
  <a href="https://shadowmalteser.itch.io/starburst" target="_blank"><!--<a href="{base}/portfolio/games/starburst">  -->
  <div>
    <img src="{base}/StarburstSS.png" alt="Screenshot of a game with a spaceship and planet in space">
    <h2>Starburst</h2>
    <p>My team's entry to the 2025 Games Fleadh, Starburst, is a fast paced 2D Shooter where you grab asteroids around you and throw them at planets to destroy them and harvest their cores.</p>
  </div>
  </a>

  <a href="https://michael-r-ryan.itch.io/unmasked" target="_blank"><!--<a href="{base}/portfolio/games/unmasked">-->
  <div>
    <img src="{base}/UnmaskedSS.png" alt="Screenshot of a game with a spaceship and planet in space">
    <h2>Unmasked</h2>
    <p>My team's entry to the 2025 Games Fleadh, Starburst, is a fast paced 2D Shooter where you grab asteroids around you and throw them at planets to destroy them and harvest their cores.</p>
  </div>
  </a>
  <a href="{base}/portfolio/games/golddivers">
  <div>
    <img src="{base}/temporary.png" alt="Screenshot of a game with a spaceship and planet in space">
    <h2>Gold Divers</h2>
    <p>My team's entry to the 2025 Games Fleadh, Starburst, is a fast paced 2D Shooter where you grab asteroids around you and throw them at planets to destroy them and harvest their cores.</p>
  </div>
  </a>
  <a href="{base}/portfolio/games/paintparty">
  <div>
    <img src="{base}/PaintPartySS.png" alt="Screenshot of a game with a spaceship and planet in space">
    <h2>Paint Party</h2>
    <p>My team's entry to the 2025 Games Fleadh, Starburst, is a fast paced 2D Shooter where you grab asteroids around you and throw them at planets to destroy them and harvest their cores.</p>
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

p {
  font-size: 20px;
}

h2 {
  font-weight: bold;
  font-size: 24px;
  color: var(--primary-color);
}

img {
  border-radius: 12px;
}

.grid {
  display: grid;
  grid-template-columns: auto auto auto;
  padding: 20px;
}

.grid div {
  padding: 15px;
}

.grid img {
  width: fit-content;
  height: fit-content;
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
  width: 90%;
  margin-bottom: 16px;
  }
}
</style>
