<script>
    import router from "page"
    import Home from "./pages/Home.svelte"
    import About from "./pages/Real_Estate_Yield_Calculator.svelte"

    let page
    router('/', () => page = Home)
    router('/Real_Estate_Yield_Calculator', () => page = About)
    router.start()
</script>

<svelte:component this={page} />