<head>
    <meta name="author" content="Riona Kelly">
</head>

<script>
// @ts-nocheck

  import { base } from '$app/paths';
  import { onMount } from 'svelte';
  
  onMount(() => {
      console.log("Contact Page Loaded");
  })
</script>

<body> 
<div class="title"><h1>Contact Me</h1></div>
<div class="first-container"> <!-- Non-functioning (for now) contact form -->
  <!-- svelte-ignore element_invalid_self_closing_tag -->
  <textarea type="text" class="name" id="name" placeholder="Name"/>
  <!-- svelte-ignore element_invalid_self_closing_tag -->
  <textarea type="text" class="email" id= "email" placeholder="Email Address"/>
</div>
<div class="second-container">
<!-- svelte-ignore element_invalid_self_closing_tag -->
<textarea type="text" class="message" placeholder="Message..."/>
<div class="third-container">
  <input type="submit" value="Submit">
</div>
<br class="desktop-only">
<br class="desktop-only">
<br class="desktop-only">
<br class="desktop-only">
<div class="fourth-container"> <!-- For some reason when i use the images the website won't load and I can'te tell why, so they must stay links for now -->
  <a href="https://www.instagram.com/rionamk/" target="_blank"> <p>Instagram</p>
    <!-- <img src="{base}/instagram.png"alt="My instagram, https://www.instagram.com/rionamk/"> -->
  </a>
  <a href="https://www.linkedin.com/in/riona-kelly-720536304/" target="_blank"><p>Linkedin</p>
    <!-- <img src="{base}/linkedin.png"  alt="My linkedin, https://www.linkedin.com/in/riona-kelly-720536304/"> -->
  </a>
  <a href="https://github.com/RionaKelly" target="_blank"><p>Github</p>
    <!-- <img src="{base}/github.png" alt="My github, https://github.com/RionaKelly"> -->
  </a>
</div>
</body>

<style>
h1 {
  grid-area: title;
  padding: 16px;
  font-weight: bold;
  font-size: 48px;
  text-align: center;
}

.first-container {
  display: flex;
  justify-content: center;
  align-items: center;
  width: 100%;
  margin: 20px 0;
}
.second-container {
  display: grid;
  justify-content: center;
  align-items: center;
  width: 100%;
  margin: 20px 0;
}
.third-container {
  display: grid;
  justify-content: center;
  align-items: center;
  width: 100%;
  margin: 20px 0;
}
.fourth-container {
  display: flex;
  justify-content: center;
  align-items: center;
  margin: 20px 0;
}

p {
  text-align: center;
  padding-right: 16px;
}

.name { /* Classes are seperated here so that i could modify them seperately and play around with them to see what its like certain ways */
  padding: 12px;
  border: 1px solid #000000;
  border-radius: 16px;
  margin-right: 6px;
  height: 45px;
  width: 200px;
  resize: none;
}
.email {
  padding: 12px;
  border: 1px solid #000000;
  border-radius: 16px;
  margin-left: 6px;
  height: 45px;
  width: 200px;
  resize: none;
  
}
.message {
  padding: 12px;
  border: 1px solid #000000;
  border-radius: 16px;
  margin-right: 0px;
  height: 250px;
  width: 500px;
  resize: vertical;
}
input[type=submit] {
  background-color: var(--primary-color);
  color: white;
  padding: 12px 20px;
  border: none;
  border-radius: 4px;
  cursor: pointer;
  padding: 12px;
  transition: 0.1s ease-in-out;
}
input[type=submit]:hover {
  background-color: var(--link-hover-color);
}

/* Mobile Navigation:*/
@media (max-width: 728px) {
  .desktop-only {
    display: none;
  }

  .first-container {
  display: grid;
  }

  .name { 
  width: 300px;
  margin-right: 0px;
  margin-bottom: 20px;

}
.email {
  width: 300px;
  margin-left: 0px;
  
}
.message {
  width: 300px;
}
}
</style>