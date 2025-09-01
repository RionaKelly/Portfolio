<script>
    // import NavigationFooter.svelte from lib folder
    import { NavigationFooter } from "$lib"
</script>

<footer>
    <!-- <h2>Riona Kelly</h2>
    <h3>Game/Web Designer & Developer</h3>-->
    <p>&copy; 2025 Riona Kelly. All rights reserved.</p>
    <!--<NavigationFooter />-->
</footer>


<style>
    footer {
        background-image: linear-gradient(rgb(7, 1, 20), rgb(13, 6, 30), rgb(19, 11, 40), rgb(13, 6, 30), rgb(7, 1, 20));
        text-align: center;
        padding: 1rem;
        color: #635286;
        position: relative;
        bottom: 0;
        width: 100%;
    }

    /*Mobile: Reduce padding for a more compact look */
    @media (max-width: 768px) {
        footer {
            padding: 0.75rem;
            position: relative;
            bottom: 0;
            font-size: 0.9rem;
        }
    }
</style>