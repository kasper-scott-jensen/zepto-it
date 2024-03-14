<script>
    import { Router, Route } from 'svelte-routing'
    import Home from './pages/Home.svelte'

    import './js/slides.min.js'
</script>

<Router>
    <Route path={'/'} component={Home} />
</Router>

<style>
  @import './css/main.css';
  @import './css/slides.min.css';
</style>