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

<h1>Privacy Policy</h1>
<p>I don't think I'm gathering any any of your information but if I am it is <b><u>NOT KNOWINGLY</u></b> and I'm definitely not using it for anything.</p>
<br>
<p>👍</p>

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