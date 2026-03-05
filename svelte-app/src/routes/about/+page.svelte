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
  <p>I'm super interested in games & art mainly, but I always love trying new things! 
    so feel free to reach out and contact me for any sort of project or opportunity, or even if you just want to talk or hang out :D.</p>
  <p class="eyes">
  <img src="{base}/eyes3.jpg" alt="Riona Kelly" class="eye">
  <img src="{base}/eyes1.jpg" alt="Riona Kelly" class="eye">
  <img src="{base}/eyes2.jpg" alt="Riona Kelly" class="eye">
  </p>
  <h2><b>The Next Part</b></h2>
  <p>Honestly I'm not sure what to put here, I don't know what people usually put in 'About Me' sections.
  <br>I also always feel weird about giving too much personal information...</p>
  <p>If you have any questions I'm happy to answer though!
  <br>For now I guess I hope you like what I've done with the place, keep looking around and I enjoyyy!!!</p>
  <p class="eyes">
  <img src="{base}/eyes3.jpg" alt="Riona Kelly" class="eye">
  <img src="{base}/eyes1.jpg" alt="Riona Kelly" class="eye">
  <img src="{base}/eyes2.jpg" alt="Riona Kelly" class="eye">
  </p>
  <h2><b>Closing Statements</b></h2>
  <p>byyyeeeee</p>
</div>

<div class="right">
<img src="{base}/riona_red.png" alt="Riona Kelly" class="pics">
<!--<br>
<img src="{base}/riona_bus.png" alt="Riona Kelly" width=600 class="pics">-->
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
 padding: 60px;
}

.pics {
  display: block;
  margin-left: auto;
  border-radius: 45px;
  max-height: 600px;
}

.eyes {
  /* display: flex;
  justify-content: center;
  align-items: center; */
  margin: 5px;
}

.eye {
  width: 32%;
  padding-right: 3px;
  border-radius: 15px;
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
    width: 100%;
    padding-left: 3px;
    padding-right: 5px;
  }

  .eye {
  border-radius: 10px;
  padding-right: 0px;
}
}
</style>