<head>
    <meta name="author" content="Riona Kelly">
</head>

<script>
// @ts-nocheck

  import { base } from '$app/paths';
  import { browser } from '$app/environment';
  import { onMount } from 'svelte';
  
  onMount(() => {
      console.log("Portfolio Showcase Page Loaded");
  })
</script>

<h1>My Portfolio Website (Right Here!!)</h1>
<p>Temporary Text</p>

<style>
p {

  padding-left: 16px;
  font-size: 24px;
  text-align: left;
}

h1 {
  grid-area: title;
  padding: 16px;
  font-weight: bold;
  font-size: 48px;
  text-align: left;
}
</style>