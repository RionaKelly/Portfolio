<script>
    // import Navigation.svelte from lib folder
    import { Navigation } from "$lib"
    import { base } from '$app/paths';
</script>


<header>
    <!-- Logo -->
    <div class="logo">
        <a href="{base}/">
            <img src="{base}/favicon2.png" alt="Website Logo">
        </a>
    </div>

    <!-- Navigation -->
    <Navigation />
</header>


<style>
    /* Header Styling */
    header {
        background-image: linear-gradient(rgb(10, 10, 10), rgb(20, 20, 20), rgb(30, 30, 30), rgb(20, 20, 20), rgb(10, 10, 10));
        display: flex; /* Enables Flexbox */
        align-items: center; /* Vertically centers the items */
        justify-content: space-between; /* Pushes logo to left, nav to right */
        color: white;
        padding: 1em;
    }

    /* Logo Container */
    .logo {
        display: flex; /* Makes logo container a Flexbox */
        align-items: center; /* Aligns text and image vertically */
    }

    .logo img {
        width: 68px;
        margin-right: 10px;
        opacity: 1;
        transition: 0.2s ease-in-out;
    }

    .logo img:hover {
        width: 60px;
        margin-right: 10px;
        opacity: 0.9;
        margin-left: 3px;
}

    /* Mobile: Center logo and stack items */
    @media (max-width: 768px) {
        header {
            flex-direction: column; /* Stacks items vertically */
            text-align: center;
        }

        .logo {
            justify-content: left;
        }
    }

</style>