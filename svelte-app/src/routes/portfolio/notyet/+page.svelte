<head>
    <meta name="author" content="Riona Kelly">
</head>

<script>
// @ts-nocheck

  import { base } from '$app/paths';
  import { browser } from '$app/environment';
  import { onMount } from 'svelte';
  
  onMount(() => {
      console.log("Not Yet Page Loaded");
  })
</script>

<div>
<div class="left">
  <h1>Sorry!</h1>
  <p>This website isn't quite ready yet! Hopefully I will have more here soon :D</p>
</div>

<div class="right">
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

/*.right img {
  margin-left: 16px;
  border-radius: 36px;
  max-height: 570px;
  filter: opacity(95%)
}

.left img {
  border-radius: 12px;
}

.icon {
  margin-top: 16px;
  margin-right: 16px;
  height: 48px;

h2 {
  font-weight: bold;
}
}*/

h1 {
  grid-area: title;
  font-weight: bold;
  font-size: 40px;
  text-align: left;
  padding-bottom: 16px;
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