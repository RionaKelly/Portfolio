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
<div>
  <div class="c1">
    <img src="{base}/StarburstSS.png" alt="Screenshot of a game with a spaceship and planet in space" width=600>
    <h2><b><a href="{base}/library">Starburst</b></h2>
    <p>My team's entry to the 2025 Games Fleadh, Starburst, is a fast paced 2D Shooter where you grab asteroids around you and throw them at planets to destroy them and harvest their cores.</p>
  </div>
  <div class="c2">
    <img src="{base}/PaintPartySS.png" alt="Screenshot of a game with 4 characters painting over an area" width=600 >
    <h2><b><a href="{base}/library">Paint Party</b></h2>
    <p>This is a multiplayer party game for up to four people where  you try and paint your colour on as much surface area as you can. I made this with 3 other students as a class project.</p>

  </div>
  <div class="c3">
    <img src="{base}/temporary.png" alt="temporary placeholder" width=600>
    <h2><b>More Soon!</b></h2>
    <p>That's all I have in store for now but I plan to update the website whenever I have more work to show off.</p>
  </div>
</div>

<style>
h1 {
  grid-area: title;
  padding: 16px;
  color: #000000;
  font-weight: bold;
  font-size: 48px;
  text-align: center;
}

p {
  padding: 16px;
}

.c1 { /* These are left as seperate classes so that I can play around and try different settings for each one */
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
}

/* Mobile Navigation:*/
@media (max-width: 1200px) {
  .right {
    display: none;
  }

  .left {
    width: 100%
  }

  .c1 {
    float: none;
    width: 100%;
  }
  .c2 {
    float: none;
    width: 100%;
  }
  .c3 {
    float: none;
    width: 100%;
  }

  .desktop-only {
    display: none;
  }
}
</style>
