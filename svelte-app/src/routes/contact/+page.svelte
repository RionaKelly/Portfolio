<head>
    <meta name="author" content="Riona Kelly">
</head>

<script>
// @ts-nocheck

  import { base } from '$app/paths';
  import { browser } from '$app/environment';
  import { onMount } from 'svelte';
  
  onMount(() => {
      console.log("Contact Page Loaded");
  })
</script>

<div class="title"><h1>Contact Me</h1></div>
<div class="first-container"> <!-- For some reason when i use the images the website won't load and I can'te tell why, so they must stay links for now -->
  <a href="mailto:rionaqueens@gmail.com" target="_blank"><p>Email</p>
    <!-- need email image here -->  
  </a>
  <br class="desktop-only">
  <a href="https://www.linkedin.com/in/riona-kelly-720536304/" target="_blank">
    <!--<img src="{base}/linkedin.png"  alt="Linkedin icon">-->
    <img src="{base}/linkedin.png" alt="Riona Kelly" width=200px>
    <p>Linkedin</p>
    <!--<img src="{base}/linkedin.png"  alt="Linkedin icon">-->
  </a>
  <br>
  <a href="https://github.com/RionaKelly" target="_blank"><p>Github</p>
    <!-- <img src="{base}/github.png" alt="My github, https://github.com/RionaKelly"> -->
  </a>
  <br class="desktop-only">
  <a href="https://www.instagram.com/rionamk/" target="_blank"> <p>Instagram</p>
    <!-- <img src="{base}/instagram.png"alt="My instagram, https://www.instagram.com/rionamk/"> -->
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

.first-container {
  margin: 20px 0;
  font-size: 32px;
}

p {
  text-align: center;
  padding-right: 16px;
}

/* Mobile Navigation:*/
@media (max-width: 728px) {
  .desktop-only {
    display: none;
  }

  .first-container {
  display: grid;
  }
}
</style>