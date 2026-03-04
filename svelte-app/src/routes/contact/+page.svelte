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
  <br class="desktop-only">
  <a href="https://www.linkedin.com/in/riona-kelly-720536304/" target="_blank">
    <p class="sink">
      <img src="{base}/linkedin.png" alt="Linkedin Icon 1">
      Linkedin
      <img src="{base}/linkedin.png" alt="Linkedin Icon 2">
    </p>
  </a>
  <br>
  <a href="https://github.com/RionaKelly" target="_blank">
    <p class="sink">
      <img src="{base}/github.png" alt="Github Icon 1">
      Github
      <img src="{base}/github.png" alt="Github Icon 2">
    </p>
  </a>
  <br>
  <a href="https://www.instagram.com/rionamk/" target="_blank">
    <p class="sink">
      <img src="{base}/instagram.png" alt="Instagram Icon 1">
      Instagram
      <img src="{base}/instagram.png" alt="Instagram Icon 2">
    </p>
  </a>
  <br>
  <div class="sink">
  <a href="mailto:rionaqueens@gmail.com" target="_blank">
    <p>
      <img src="{base}/mail.png" alt="Email Icon 1">
      Email 
      <img src="{base}/mail.png" alt="Email Icon 2">
    </p>
    <p class="email">(rionaqueens@gmail.com)</p>
  </a>
  </div>
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
  margin: 10px 0;
  font-size: 32px;
}

p {
  text-align: center;
}

img {
  width: 24px;
}

.email {
  font-size: 12px;
  margin: 0px;
}
.sink {
  transition: 0.1s ease-in-out;
}

.sink:hover {
        text-shadow: 0 2px 3px rgba(0, 0, 0, 0.15);
        transform: translateY(1px);
}

/* Mobile Navigation:*/
@media (max-width: 728px) {
  .first-container {
  display: grid;
  font-size: 28px;
  }

  img {
  width: 20px;
  }
}
</style>