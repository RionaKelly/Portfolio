<head>
    <meta name="author" content="Riona Kelly">
</head>

<script>
// @ts-nocheck

  import { base } from '$app/paths';
  import { onMount } from 'svelte';
  
  onMount(() => {
      console.log("Home Page Loaded");
  })
</script>

<div class="first-div">
  <div class="left">
    <p>Hey! I'm Riona, nice to meet you!!</p>
    <div class="mobile-only">
    <img src="{base}/riona_purple.png" alt="Riona under purple lighting">
    </div>
    <p>Here you can see my work and learn more about me. 
    <br>Recently I've been working on a new project for this college semester, a Desktop Pet!</p>
    <div class="pet_div">
    <img src="{base}/pets.gif" class="pets" alt="Desktop Pets wandering around screen">
    </div>
    <p>I have wanted to make something like this for a really long time and I'm so glad that I finally get the opportunity! 
      As of right now there are 3 pets that you can start with and they will just wander around your screen, sometimes stopping and looking at you or sitting down.</p>
    <p>Eventually I plan to make it function more similarly to a <i>Tamagotchi</i> or <i>Digimon</i> where you take care of and raise your pet until they are old enough to leave. 
      You can download the current prototype and read more about this project <a href="{base}/portfolio/games/desktoppet"><b>here</b></a>, keep an eye out for future updates! :D</p>
    <p>Hope you enjoy looking around, and if you'd like to contact me for any reason you can find out how on the <a href="{base}/contact"><b>Contact</b></a> page, and checkout my Github below to see the code for all of my projects.</p>
    <a href="https://github.com/RionaKelly" target="_blank"><img src="{base}/github_link.png" class="left-padding" alt="My github link, https://github.com/RionaKelly"></a>
  <h1>Recent Work</h1>
  </div>
  <div class="right">
    <img src="{base}/riona_purple.png" alt="Riona Kelly" class="desktop-only" width="800">
  </div>
</div>


<div class="second-div">
<div class="left">
<h2><u>Starburst</u></h2>
<p>This is my most recent and proudest  project right now, <i><b>Starburst</b></i>. 
  I made it with a friend for the <u>2025 Games Fleadh</u>, and we were awarded <u><i>Best Game using Libraries</i></u> and <u><i>Best Game Mechanics</i></u>. 
  It is a fast paced 2D Shooter where you grab asteroids flying past you and throw them at planets to destroy them and harvest their cores. 
  <br>I co-designed this with my friend and created the assets and sounds, while he coded everything for it.</p>
  <p>Check out the Trailer below! You can also read more about it on my website <a href="{base}/portfolio/games/starburst"><b>here</b></a> or visit the <a href="https://shadowmalteser.itch.io/starburst" target="_blank"><b>itch page</b></a> if you'd like to try it out.</p>
<div class="iframe_scale"><iframe title="Starburst" src="https://www.youtube.com/embed/gC9f7HGMo1s?si=jWfad7fnDouoU-tT" class="second-content" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen frameborder="0"></iframe></div>
</div>
<div class="right">
<h2><u>An Phiast In: Fishy Business</u></h2>
<p>This is my team's Game Sting submisson for the <u>2026 Dingle Animation Festival</u>!
  It's a short comedic detective game where an amnesiac An Phiast (the festival's mascot) must try to solve the mystery of who stole 'The Perfect Fish and Chips' from the local chippers. 
  You'll meet a colourful cast of characters to help you on your journey and gather evidence to try and find the culprit.
  We worked as a team to design everything during the game's development, and I wrote and implemented the dialogue, created menus, and modelled the indoor area.</p>
  <p>You can visit the <a href="https://shadowmalteser.itch.io/https://shadowmalteser.itch.io/fishybusiness" target="_blank"><b>itch page</b></a> to try it or read a little more on my website <a href="{base}/portfolio/games/fishybusiness"><b>here</b></a>.</p>
  <img src="{base}/FishyBusinessCover.png" class="second-content" alt="Green monster in detective outfit with chip shop owner and the title 'An Phiast in: Fishy Business'">
</div>
</div>

<div class="third-div">
<p>For my older projects check out the <a href="{base}/portfolio"><b>Portfolio</b></a> page, most of them are just old college projects that I'm not a big fan of anymore but it's nice to document them anyway.</p>
<h1>Note from the Author</h1>
  <p>I'm really happy with this website but there's still so much more I want to do with it to make it more me, I hope I can keep adding to it when I have the free time because it's a really fun way to express myself.
    I'm trying to focus as much as I can right now on my current college project (the Desktop Pet (please check it out again it's so cool and I'm really proud of it)) 
    so I don't have the time but one day I'll come back and update this place again. 
    <br> Also hi anyone looking at this from the Animation Festival :D I am working on this as fast as I can so that it will be ready in time for that.
  </p>
  <p>This website was last updated on 9/3/2026</p>
</div>

<style>
p {
  padding-top: 4px;
  padding-left: 20px;
  font-size: 24px;
  text-align: left;
  margin-right: 8px;
}

h1 {
  grid-area: title;
  padding: 16px;
  padding-bottom: 0px;
  margin-top: 8px;
  font-weight: bold;
  font-size: 40px;
  text-align: left;
}

h2 {
  font-weight: bold;
  font-size: 28px;
  padding-left: 20px;
}

.iframe_scale {
  height: 56.25%;
}

iframe {
  width: 100%;
  height: 100%;
}

.second-content{
  padding: 20px;
  border-radius: 42px;
}

.left-padding {
  margin-left: 20px;
}

.pets {
  margin-left: 20px;
  width: 1180px;
}

.left {
 float: left;
}

.right {
 float: right;
}

.first-div .left {
 width: 65%;
}
.first-div .right {
 width: 35%;
 margin-left: 16px;
}
.second-div .left {
 width: 50%;
}
.second-div .right {
 width: 50%;
}

.first-div .right img{
  margin-left: auto;
  border-radius: 45px;
  padding: 16px;
  padding-top: 2%;
  padding-left: 2%;
}

.first-div .left img{
  border-radius: 16px;
}

.mobile-only{
  display: none;
  margin: 12px;
}

.mobile-only img {
  border-radius: 45px;
}

.pet_div {
  margin-right: 30px;
}

.first-div {
  padding: 6px;
  padding-top: 16px;
  display: flex;
  padding-left: 16px;
}
.second-div {
  display: flex;
  padding-left: 16px;
}
.third-div {
  padding: 8px;
  padding-left: 16px;
}

/* Mobile Navigation:*/
@media (max-width: 1000px) {
    .first-div {
    padding-left: 4px;
  }
  .second-div {
    padding-left: 4px;
  }
  .third-div {
    padding-left: 4px;
  }
  
  p {
    font-size: 22px;
  }

  .first-div .right {
    display: none;
  }
    .first-div .left {
    width: 100%;
  }

  .pets {
    margin-left: 20px;
    width: 100%;
  }

  .second-div{
    display: block;
  }

  .second-div .left {
    width: 100%;
    float: none;
  }
  .second-div .right {
    width: 100%;
    float: none;
  }
  .mobile-only{
    display: block;
  }
  .mobile-only img {
    border-radius: 36px;
  }
}
</style>