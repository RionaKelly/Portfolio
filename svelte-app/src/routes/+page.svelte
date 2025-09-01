<head>
    <meta name="author" content="Riona Kelly">
</head>

<script>
// @ts-nocheck

  import { base } from '$app/paths';
  import { onMount } from 'svelte';
  
  onMount(() => {
      console.log("Home Page Loaded");
  })
</script>

<div class="first-div">
  <div class="left">
    <p>Hey! I'm Riona, nice to meet you!! <br> I'm a 20 year old Irish woman studying Game & Web Design.</p>
    <p>Here you can see my work and learn more about me. This is my most recent and proudest project right now, <i>Starburst</i>. I made it with a friend for the 2025 Games Fleadh, and we were awarded Best Game using Libraries and Best Game Mechanics.</p>
    <iframe width="560" height="315" class="left-padding" title="Starburst" src="https://www.youtube.com/embed/gC9f7HGMo1s?si=jWfad7fnDouoU-tT" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen frameborder="0"></iframe>
    <br>
    <a href="https://github.com/RionaKelly" target="_blank"><img src="{base}/github_link.png" class="left-padding" alt="My github link, https://github.com/RionaKelly"></a>
    <p>Hope you enjoy looking around, and if you want to contact me for any reason you can find out how on the <a href="{base}/contact">Contact</a> page. I love meeting new people if you ever want to talk for any reason!</p>
  </div>
  <div class="right" align="right">
    <img src="{base}/riona_purple.png" alt="Riona Kelly" class="desktop-only" width="800">
  </div>
</div>
<br>
<h1>My Recent Work</h1>
<div class="second-div">
  <div class="showcase1">
    <img src="{base}/StarburstSS.png" alt="Screenshot of a game with a spaceship and planet in space" width=600>
    <h2><b><a href="{base}/library">Starburst</b></h2>
    <p>My team's entry to the 2025 Games Fleadh, Starburst, is a fast paced 2D Shooter where you grab asteroids around you and throw them at planets to destroy them and harvest their cores.</p>
  </div>
  <div class="showcase2">
    <img src="{base}/PaintPartySS.png" alt="Screenshot of a game with 4 characters painting over an area" width=600 >
    <h2><b><a href="{base}/library">Paint Party</b></h2>
    <p>This is a multiplayer party game for up to four people where  you try and paint your colour on as much surface area as you can. I made this with 3 other students as a class project.</p>

  </div>
  <div class="showcase3">
    <img src="{base}/temporary.png" alt="temporary placeholder" width=600>
    <h2><b>More Soon!</b></h2>
    <p>That's all I have in store for now but I plan to update the website whenever I have more work to show off.</p>
  </div>
</div>

<style>

p {
  padding-top: 16px;
  padding-left: 16px;
  font-size: 24px;
  text-align: left;
}

h1 {
  text-align: left;
  padding-left: 16px;
}

.left-padding {
  padding-left: 20px;
}

.left {
 float: left;
 width: 50%;
}
.right {
 float: right;
 width: 50%;
 padding: 16px;
 max-height: 200px;
}

.first-div {
  padding-top: 16px;
  display: flex;
}
.second-div {
  padding: 8px;
}

.showcase1 { /* These are left as seperate classes so that I can play around and try different settings for each one */
  float: left;
  width: 33%;
  padding: 16px;
}
.showcase2 {
  float: left;
  width: 33%;
  padding: 16px;
}
.showcase3 {
  float: right;
  width: 33%;
  padding: 16px;
}
.showcase1 p {
  padding-left: 0;
}
.showcase2 p {
  padding-left: 0;
}
.showcase3 p {
  padding-left: 0;
}

/* Mobile Navigation:*/
@media (max-width: 1200px) {
  .right {
    display: none;
  }

  .left {
    width: 100%
  }

  .showcase1 {
    float: none;
    width: 100%;
  }
  .showcase2 {
    float: none;
    width: 100%;
  }
  .showcase3 {
    float: none;
    width: 100%;
  }

  .desktop-only {
    display: none;
  }
}
</style>