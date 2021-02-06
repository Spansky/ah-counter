<script>
    import Router from 'svelte-spa-router'
    import AhCounter from './AhCounter.svelte';
    import ResultPage from './ResultPage.svelte';

    const routes = {
        '/' : AhCounter,
        '/results' : ResultPage,
    }
</script>

<body>
    <Router {routes}/>
</body>
