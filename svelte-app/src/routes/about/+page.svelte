<head>
    <meta name="author" content="Riona Kelly">
</head>

<script>
// @ts-nocheck
    import { base } from '$app/paths';
    import { browser } from '$app/environment';
    import { onMount } from 'svelte';

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
<div class="row">
<div class="left">
  <h1>About Me</h1>
  <p>Hello!! I'm Riona, a Web/Game Designer and Developer based in Ireland :></p>
  <p>I'm super interested in games, art and poetry, and am always up for a challenge or to try something new.
  <br>So feel free to reach out and contact me for any sort of project or opportunity!</p>
  <p></p>
  <h2><b>Some Random Facts</b></h2>
  <p>- If you couldn't tell, my favourite colours are purple and yellow.</p>
  <p>- I have 3 cats</p>
  <p>- I've been making games since I was a kid, they weren't very good back then but hopefully they're better now!!</p>
  <p>- I loove socialising and will take any opportunity to meet new people (a lot of you reading this are probably random people I met while out, nice to see you again!)</p>
  <p>- I'm hypermobile/double-jointed and can bend my my body in ways that it probably shouldn't go!</p>
  <p>- I love cosplaying and you can find me at most Irish conventions if I have the money for them.</p>
</div>

<div class="right" align="right">
<div class="carousel">{#if Carousel}
 <Carousel
     bind:this={carousel}
     autoplay
     autoplayDuration={3000}
     pauseOnFocus
     swiping
     dots={false}
    let:showPrevPage
    let:showNextPage
 >
     <div><center>
      <img src="{base}/riona_red.png" alt="Riona Kelly" width=700>
      </center></div>
     <div><center>
      <img src="{base}/riona_purple.png" alt="Riona Kelly" width=700>
      </center></div>
     <div><center>
      <img src="{base}/riona_bus.png" alt="Riona Kelly" width=700>
      </center></div>
 </Carousel>
{:else}
 Fallback content while loading
 <p>Loading carousel...</p>
{/if}</div>
</div>
</div>
 

<style>

.left {
 float: left;
 width: 50%;
}
.right {
 float: right;
 width: 50%;
 padding: 42px;
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
    float:left;
    width: 500px;
  }

  .left {
    width: 100%
  }
}
</style>