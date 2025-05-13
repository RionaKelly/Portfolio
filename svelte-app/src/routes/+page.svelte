<head>
    <meta name="author" content="Riona Kelly">
</head>

<script>
// @ts-nocheck

  import { base } from '$app/paths';
  import { onMount } from 'svelte';
  import { browser } from '$app/environment';

  /**
 * @type {__sveltets_2_IsomorphicComponent<__sveltets_2_PropsWithChildren<{ timingFunction?: string | undefined; arrows?: boolean | undefined; infinite?: boolean | undefined; initialPageIndex?: number | undefined; duration?: number | undefined; autoplay?: boolean | undefined; autoplayDuration?: number | undefined; autoplayDirection?: any; pauseOnFocus?: boolean | undefined; autoplayProgressVisible?: boolean | undefined; dots?: boolean | undefined; swiping?: boolean | undefined; particlesToShow?: number | undefined; particlesToScroll?: number | undefined; goTo?: ((pageIndex: any, options: any) => Promise<void>) | undefined; goToPrev?: ((options: any) => Promise<void>) | undefined; goToNext?: ((options: any) => Promise<void>) | undefined; }, { prev: { showPrevPage: any; }; default: { loaded: any[]; currentPageIndex: any; }; next: { showNextPage: any; }; dots: { currentPageIndex: any; pagesCount: number; showPage: (pageIndex: any) => Promise<void>; }; }>, { [evt: string]: CustomEvent<any>; }, { prev: { showPrevPage: any; }; default: { loaded: any[]; currentPageIndex: any; }; next: { showNextPage: any; }; dots: { currentPageIndex: any; pagesCount: number; showPage: (pageIndex: any) => Promise<void>; }; }, { goTo: (pageIndex: any, options: any) => Promise<void>; goToPrev: (options: any) => Promise<void>; goToNext: (options: any) => Promise<void>; }, string>}
 */
  let Carousel; // for dynamic import of the carousel component
  /* @type {import('svelte-carousel').default} */
  let carousel; // for calling methods of the carousel instance
  
  onMount(async () => {
      console.log("Home Page Loaded");
      if (browser) {
          // dynamically import only in the browser
          const module = await import('svelte-carousel');
          Carousel = module.default;
      }
  });
</script>
<div class="first-div">
  <div class="left">
    <p>Hey! I'm Riona, nice to meet you!!</p>
    <iframe width="560" height="315" class="left-padding" title="Starburst" src="https://www.youtube.com/embed/gC9f7HGMo1s?si=jWfad7fnDouoU-tT" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen frameborder="0"></iframe>
    <br>
    <a href="https://github.com/RionaKelly" target="_blank"><img src="{base}/github_link.png" class="left-padding" alt="My github link, https://github.com/RionaKelly"></a>
    <p>Here you can see my recent work and learn more about me. Hope you enjoy! :D</p>
  </div>
  <div class="right" align="right">
    <img src="{base}/riona_purple.png" alt="Riona Kelly">
  </div>
</div>
<div>
  <p>test paragraph 1</p>
</div>
<p>test paragraph 2</p>

<!-- <div class="carousel">{#if Carousel}         Leaving this here in case I need a carousel example for later
 <Carousel
     bind:this={carousel}
     autoplay
     autoplayDuration={5000}
     autoplayProgressVisible
     pauseOnFocus
     swiping
 >
     <div><center>
      <img src="{base}/grape.png" alt="Blueberry Lavender Tea Cans" width="300" height="200">
      <h2>Blueberry Lavender</h2></center></div>
     <div><center>
      <img src="{base}/doctor.png" alt="Elderflower" width="300" height="200">
      <h2>Elderflower</h2></center></div>
     <div><center>
      <img src="{base}/cherry-vanilla.png" alt="Cherry Blossom" width="300" height="200">
      <h2>Cherry Blossom</h2></center></div>
 </Carousel>
{:else}
 Fallback content while loading
 <p>Loading carousel...</p>
{/if}</div> -->

<style>

p {
  padding-top: 16px;
  padding-left: 16px;
  font-size: 24px;
  text-align: left;
}

iframe {

}

.left-padding {
  padding-left: 20px;
}

.left {
 float: left;
 width: 50%;
}
.right {
 float: right;
 width: 50%;
 padding: 16px;
 max-height: 200px;
}

.first-div {
  padding-top: 16px;
  display: flex;
}
</style>