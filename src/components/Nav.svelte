<script>
    import Menu from '../assets/svg/Menu.svelte'
    import Logo from '../assets/svg/Logo.svelte'
</script>

<header>
    <nav>
        <span>
            <Logo />
        </span>
        <span>
            <Menu />
        </span>
    </nav>
    <div />
</header>

<style lang="scss">
    nav {
        z-index: 10;
        position: fixed;
        top: 0;
        // min-width: fit-content;
        width: 100%;
        display: flex;
        justify-content: space-between;
        align-items: flex-end;
        padding: 6em 10em 0 10em;
        // max-width: 2300px;
        max-width: 100vw;
        margin: 0 auto;
        mix-blend-mode: difference;
        @media screen and (max-width: 1024px) {
            padding: 4em 2em 0 2em;
        }
    }
    div {
        width: 100%;
        height: 160px;
    }
</style>
