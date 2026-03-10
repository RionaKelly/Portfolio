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

<div>
<div class="left">
  <h1>Desktop Pet</h1>
  <p>Explanation</p>
  <p>What's Next</p>
  <p>Links</p>
  <img src="{base}/itchio.png" alt="clickable itch.io icon">

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
  margin-left: auto;
  border-radius: 45px;
  max-height: 570px;
  filter: opacity(95%)
}

.left img {
  padding-top: 16px;
}

h1 {
  grid-area: title;
  font-weight: bold;
  font-size: 40px;
  text-align: left;
  padding-bottom: 16px;
}

/*h2 {
  padding-left: 16px;
  padding-bottom: 2px;
}*/

p {
  font-size: 20px;
}

/* Mobile Navigation:*/
@media (max-width: 1200px) {
  .right {
    width: 100%;
    padding: 10px;
    padding-left: 20px;
    padding-right: 20px;
  }

  .left {
    width: 100%;
    padding-left: 3px;
    padding-right: 5px;
  }
}
</style>