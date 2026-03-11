<head>
    <meta name="author" content="Riona Kelly">
</head>

<script>
// @ts-nocheck

  import { base } from '$app/paths';
  import { browser } from '$app/environment';
  import { onMount } from 'svelte';
  
  onMount(() => {
      console.log("Desktop Pet Page Loaded");
  })
</script>

<div>
<div class="left">
  <h1>Desktop Pet</h1>
  <p>This is a virtual pet that will live on your computer desktop that I am working on as part of my full time college project! 
  <br>When you start the game you will gain a random pet that you can take care of and raise by feeding and playing with them while they keep you company, 
  until they are old enough to leave and for the internet to go on their own adventure!</p>
  <h2>What's New</h2>
  <p>I just added 2 more pets to the game! You can now start with a Bird, Bunny, or Octopus!</p>
  <h2>What's Next</h2>
  <p>I've been having some issues getting certain features I want working so the next update is taking longer than expected :(
  <br>For some reason I just cannot make the transparent pixels click-throughable. I'll figure it out. Then I'll be working on moving the pet around and a UI.</p>
  <h2>Known Issues</h2>
  <p>- The Pet will only function on your left monitor if you have multiple.</p>

   <a href="https://rionakelly.itch.io/desktoppet" target="_blank"><img src="{base}/itchio.png" alt="clickable itch.io icon"></a>
    <a href="https://github.com/RionaKelly/DesktopPet" target="_blank"><img src="{base}/github.png" alt="clickable github icon"></a>
</div>

<div class="right">
<img src="{base}/DesktopPetSS.png" alt="Screenshot of pixelated animals on a computer desktop">
</div>
</div>

<style>

.left {
 float: left;
 width: 60%;
 padding-left: 36px;
 padding-top: 16px;
}

.right {
 float: right;
 width: 40%;
 padding: 60px;
 padding-top: 4%
}

.right img {
  margin-left: 16px;
  border-radius: 45px;
  max-height: 570px;
  filter: opacity(95%)
}

.left img {
  margin-top: 16px;
  margin-right: 16px;
  height: 48px;
}

h1 {
  grid-area: title;
  font-weight: bold;
  font-size: 40px;
  text-align: left;
  padding-bottom: 16px;
}

h2 {
  font-weight: bold;
}

p {
  font-size: 20px;
}

/* Mobile Navigation:*/
@media (max-width: 1200px) {
  .left {
    width: 100%;
    padding-left: 24px;
    padding-right: 24px;
  }
  
  .right {
    width: 100%;
    padding: 10px;
    padding-left: 24px;
    padding-right: 24px;
  }
}
</style>