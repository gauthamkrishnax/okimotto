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
</header>

<style lang="scss">
    header {
        position: fixed;
        top: 0;
        left: 0;
        right: 0;
        nav {
            display: flex;
            justify-content: space-between;
            align-items: flex-end;
            padding: 6em 10em 0 10em;
        }
    }
</style>
