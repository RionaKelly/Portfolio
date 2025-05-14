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

</style>
