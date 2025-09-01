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
      console.log("Library Page Loaded");
      if (browser) {
          // dynamically import only in the browser
          const module = await import('svelte-carousel');
          Carousel = module.default;
      }
  });
</script>
<h1>Paint Party</h1>
<p>Temporary Text</p>

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