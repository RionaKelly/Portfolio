<head>
    <meta name="author" content="Riona Kelly">
</head>

<script>
// @ts-nocheck

  import { base } from '$app/paths';
  import { browser } from '$app/environment';
  import { onMount } from 'svelte';
  
  onMount(() => {
      console.log("About Page Loaded");

  let randomNumber = Math.floor(Math.random() * 2) + 1;
  
  if (randomNumber == 1) {
       document.getElementById("pic1").style.display = "block";
   }
  if (randomNumber == 2) {
       document.getElementById("pic2").style.display = "block";
   }
  //if (randomNumber == 3) {
       //document.getElementById("pic3").style.display = "block";
   //}
  });
</script>

<div>
<div class="left">
  <h1>About Me</h1>
  <p>Hello!! I'm Riona, a Web/Game Designer & Developer based in Ireland :></p>
  <p>I'm super interested in games mainly, but I love art and poetry, and always enjoy trying new things! 
  So feel free to reach out and contact me for any sort of project or opportunity, or even if you just want to talk or hang out :D.</p>
  <p class="eyes">
  <img src="{base}/eyes3.jpg" alt="First Eyes for Seperation" class="eye">
  <img src="{base}/eyes1.jpg" alt="Second Eyes for Seperation" class="eye">
  <img src="{base}/eyes2.jpg" alt="Third Eyes for Seperation" class="eye">
  </p>
  <h2><b>I Love Organisation but Can't Think of a Title</b></h2>
  <p>Honestly I'm not sure what to put here, I don't know what people usually put in 'About Me' sections,
    and I always feel weird about giving too much personal information. I'll fill this up properly eventually maybe but for now 
    feel free to message me if you have any questions or want to get to know me more!</p>
  <p>If you can't tell by now, I'm not the most professional person. I can be when I want to and sometimes it's fun, 
    but I believe that my work (or solo work at least) should be an expression of myself, and that anything less fun and silly just isn't personal enough. 
    It wouldn't be Riona.</p>
  <p>Thank you for reading and visiting my website, I hope you like what I've done with the place and enjoy your look around!</p>
  <p class="eyes">
  <img src="{base}/eyes3.jpg" alt="First Eyes for Seperation" class="eye">
  <img src="{base}/eyes1.jpg" alt="Second Eyes for Seperation" class="eye">
  <img src="{base}/eyes2.jpg" alt="Third Eyes for Seperation" class="eye">
  </p>
  <h2><b>Bonus!!!</b></h2>
  <p>I'm too indecesive to ever choose a photo for anything so the image here will randomise between some set choices (woah!!) (so cool!!!)</p>
</div>

<div class="right">
<img src="{base}/riona_red.png" alt="Red Riona Selfie with Face Markings" id="pic1">
<img src="{base}/riona_bus.png" alt="Riona Selfie at a Bus Stop" id="pic2">
<img src="{base}/riona_purple.png" alt="Purple Riona Selfie" id="pic3"> <!-- Disabled for now because I don't like it -->
</div>
</div>

<style>

.left {
 float: left;
 width: 60%;
 padding-left: 20px;
}

.right {
 float: right;
 width: 40%;
 padding: 60px;
 padding-top: 8%
}

.right img{
  display: none;
  margin-left: auto;
  border-radius: 45px;
  max-height: 570px;
  filter: opacity(95%)
}

.eyes {
  /* display: flex;
  justify-content: center;
  align-items: center; */
  margin: 5px;
}

.eye {
  width: 30%;
  border-radius: 15px;
  margin: 5px;
  filter: opacity(100%);
}

h1 {
  grid-area: title;
  padding: 16px;
  font-weight: bold;
  font-size: 40px;
  text-align: left;
}

h2 {
  padding-left: 16px;
  padding-bottom: 2px;
}

p {
  padding-left: 16px;
  font-size: 20px;
}

/* Mobile Navigation:*/
@media (max-width: 1200px) {
  .right {
    display: block;
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

  .eye {
  border-radius: 10px;
  padding-right: 0px;
}
}
</style>