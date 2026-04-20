<head>
    <meta name="author" content="Riona Kelly">
</head>

<script>
// @ts-nocheck

  import { base } from '$app/paths';
  import { browser } from '$app/environment';
  import { onMount } from 'svelte';
  
  onMount(() => {
      console.log("Desktop Pet Page Loaded");
  })
</script>

<div>
<div class="left">
  <h1>Desktop Pet</h1>
  <p>This is a simple virtual pet that I am making for my college project. They will live on your desktop while you can raise and take care of them until they are old enough to leave. This game is intended to be something that sits on your screen or side-monitor while you do other things, keeping your company and every now and then looking for attention.</p>
  <p>This is still a work-in-progress but feel free to download and enjoy my silly creature from the itch.io link at the bottom of the page! If you have any thoughts just let me know, good or bad I don't mind I would love to hear!!</p>
  <img src="{base}/pets.gif" class="left-padding" alt="Desktop Pets wandering around screen" width=1180px>
  <h2>What's In?</h2>
  <p>So far you can start with one of three random Pets when you open the game, and they will wander around your desktop;&nbsp;stopping, starting, sitting, and staring. You can throw them around the screen which is really fun I would highly recommend this.</p>
  <p>Clicking on your Pet will open a menu, here you can view a little info about the game or your pet, change settings, and exit the game (ignore the ugly parts in the UI its a work in progress). If you want your Pet confined to a different monitor than the starting one just drag them over there :&gt;</p>
  <p>As your pet grows up they will have a chance to evolve (after 5, 15, and 30 hours), when evolving a pet will get bigger and have a chance of gaining a new colour palette, this will also effect the menu's looks. Your pet's data will be saved every minute or when you close the app, if you want to restart or try to get a different pet just turn off saving and delete your data in the settings.</p>
  <h2>Controls/Instructions</h2>
  <p>Left Click - Stops the pet in place<br>Hold Left Click - Drags the pet around so you can move or throw them<br>Double Left Click - Opens the Menu<br>(Not in yet) Right Click - Pet your pet :)</p>
  <p>In the Menu you can access a few pages:<br>
  - <strong>Your Pet:</strong>&nbsp;Where you can view info about your pet and change their name.<br>
  - <strong>Info:</strong>&nbsp;Where you can get a small refresher on the game and controls, I'll make this more in depth eventually.<br>
  - <strong>Settings:</strong>&nbsp;Where&nbsp; you can modify game settings, here you can Silent the game, enable larger hitboxes, turn on a wobbly shader for that Tamagotchi vibe, disable the menu opening automatically, and turn off saving/delete data for those who want to reset for their favourite pet.<br>
  - <strong>Exit:</strong>&nbsp;Which will save and close the game, just closing the window manually will do this too.<br>
  - You can also close this menu with the top right button.</p>
  <h2>What's Next</h2>
  <p>Next up I need to actually implement the happiness and fullness mechanic so that you can take care of the pet rather than just watching them, this will include the Shop and Game menus. After that its mainly polishing, fixing bugs, and just making it all better for my project deadline. I will also add petting :).</p>
  <h2>Known Issues</h2>
  <p>- There are some stray pixels outside of clickable area on some monitors, I think that this is a monitor issue that I don't seem to be able to do anything about.<br>
    - Font should be made more readable, give option to increase window size too for better visibility.<br>
    - I gotta optimise generally I think as I've heard of issues from some people about lag sometimes or extra battery usage</p>
   <a href="https://rionakelly.itch.io/desktoppet" target="_blank"><img src="{base}/itchio.png" class="icon" alt="clickable itch.io icon"></a>
    <a href="https://github.com/RionaKelly/DesktopPet" target="_blank"><img src="{base}/github.png" class="icon" alt="clickable github icon"></a>
</div>

<div class="right">
<img src="{base}/DesktopPetSS.png" alt="Screenshot of pixel-art animals on a computer desktop">
<img src="{base}/pet_menu.png" alt="Screenshot of pixel-art animals with a menu with options above them"> 
<img src="{base}/pet_pattern.png" alt="Screenshot of pixel-art orange octopus"> 
<img src="{base}/pet_theme.png" alt="Screenshot with pixel-art octopus and menu from prior images but recoloured in a restro pastel aesthetic">
<img src="{base}/pet_ideas.png" alt="Twelve pixel-art animals from my project">
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
}

h1 {
  grid-area: title;
  font-weight: bold;
  font-size: 40px;
  text-align: left;
  padding-bottom: 16px;
}

h2 {
  font-weight: bold;
  font-size: 28px;
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