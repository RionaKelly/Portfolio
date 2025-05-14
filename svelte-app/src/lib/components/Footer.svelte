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
        background-image: linear-gradient(rgb(10, 10, 10), rgb(20, 20, 20), rgb(30, 30, 30), rgb(20, 20, 20), rgb(10, 10, 10));
        color: white;
        text-align: center;
        padding: 1rem;
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