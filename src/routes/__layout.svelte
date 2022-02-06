<script>
    import '../app.css'
    import Nav from '../components/nav.svelte'
    import Search from '../components/search.svelte'
</script>

    
<main class="flex">
    
     <Nav/>
    <div >
    <Search/>
        <slot><!-- optional fallback --></slot>
    </div>
</main>
