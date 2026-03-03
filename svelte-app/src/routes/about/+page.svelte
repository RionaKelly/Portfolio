<head>
    <meta name="author" content="Riona Kelly">
</head>

<script>
// @ts-nocheck

  import { base } from '$app/paths';
  import { browser } from '$app/environment';
  import { onMount } from 'svelte';
  
  onMount(() => {
      console.log("Home Page Loaded");
  })
</script>

<div class="row">
<div class="left">
  <h1>About Me</h1>
  <p>Hello!! I'm Riona, a Web/Game Designer & Developer based in Ireland :></p>
  <p>I'm super interested in games, art and poetry, and am always up for a challenge or to try something new.
  <br>So feel free to reach out and contact me for any sort of project or opportunity!</p>
  <p class="eyes">
  <img src="{base}/eyes3.jpg" alt="Riona Kelly" class="eye">
  <img src="{base}/eyes1.jpg" alt="Riona Kelly" class="eye">
  <img src="{base}/eyes2.jpg" alt="Riona Kelly" class="eye">
  </p>
  <h2><b>Some Random Facts</b></h2>
  <p>- If you couldn't tell, my favourite colours are purple and yellow.</p>
  <p>- I have 3 cats</p>
  <p>- I've been making games since I was a kid, they weren't very good back then but hopefully they're better now!!</p>
  <p>- I loove socialising and will take any opportunity to meet new people (a lot of you reading this are probably random people I met while out, nice to see you again!)</p>
  <p>- I'm hypermobile/double-jointed and can bend my my body in ways that it probably shouldn't go!</p>
  <p>- I love cosplaying and you can find me at most Irish conventions if I have the money for them.</p>
  <p class="eyes">
  <img src="{base}/eyes3.jpg" alt="Riona Kelly" class="eye">
  <img src="{base}/eyes1.jpg" alt="Riona Kelly" class="eye">
  <img src="{base}/eyes2.jpg" alt="Riona Kelly" class="eye">
  </p>
</div>

<div class="right">
<img src="{base}/riona_red.png" alt="Riona Kelly" width=600 class="pics">
<br>
<img src="{base}/riona_bus.png" alt="Riona Kelly" width=600 class="pics">
</div>
</div>
<div>

</div>

<style>

.left {
 float: left;
 width: 50%;
 padding-left: 20px;
}
.right {
 float: right;
 width: 50%;
 padding: 40px;
 float: right;
}

.pics {
  display: block;
  margin-left: auto;
}

.eyes {
  display: flex;
  justify-content: center;
  align-items: center;
}

.eye {
  width: 33%;
}

.row:after {
 content: "";
 display: table;
 clear: both;
}

h1 {
  grid-area: title;
  padding: 16px;
  font-weight: bold;
  font-size: 48px;
  text-align: left;
}

h2 {
  padding-left: 16px;
  padding-bottom: 8px;
}

p {
  padding-left: 16px;
  font-size: 18px;
}

/* Mobile Navigation:*/
@media (max-width: 1200px) {
  .right {
    display: none;
  }

  .left {
    width: 100%
  }
}
</style>