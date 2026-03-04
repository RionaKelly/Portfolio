<script>
    import { base } from '$app/paths';
</script>


<nav>
    <ul> 
        <li><p>&copy; 2026 Riona Kelly. All rights reserved.</p></li>
        <li><a href="{base}/privacy" style="color: #635286;">Privacy Policy</a></li>
    </ul>
</nav>

<style>
    nav ul {
        list-style: none;
        padding: 0;
        margin: 0;
        display: flex;
        justify-content: center;
    }

    nav ul li {
        margin: 0 15px;
    }

    nav ul li a {
        text-decoration: none;
        font-weight: bold;
    }

    /* Only on Desktop: */
@media (min-width: 728px) {
    nav ul li {
        width: 300px;
    }
}

    /* Only on Mobile:
@media (min-width: 728px) {
    .desktop-only {
    display: none;
  }
} */
</style>