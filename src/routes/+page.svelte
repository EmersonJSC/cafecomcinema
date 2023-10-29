<script>
    import { onMount } from 'svelte';
    import axios from 'axios';
    import Index from './index/+page.svelte'

    let movies = [];
    
    onMount(async () =>{
        const APIKey = 73e51399
        try {
            const response = await axios.get(`http://www.omdbapi.com/?s=movie&type=movie&r=json&page=100&apikey=73e51399&`);
            movies = response.data.Search;
            console.log(response.data);
        } catch (error) {
            console.error(error);
        }
    });
</script>

<Index />

<style>
    :global(body){
        margin: 0px;
        padding: 0px;
    }
</style>
