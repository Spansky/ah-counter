<script>
import Speaker from './components/Speaker.svelte';
let speakers = 1;

function handleClick(){
    speakers += 1;
}

</script>

<style>
    button {
        width: 100%;
    }
</style>

<h1>Ah-Counter</h1>

<table>
    <thead>
        <tr>
            <th>Name</th>
            <th>Ah</th>
            <th>Um</th>
            <th>Er</th>
            <th>Well</th>
            <th>So</th>
            <th>Like</th>
            <th>But</th>
            <th>Repeats</th>
            <th>Other</th>
        </tr>
    </thead>
    <tbody>
        {#each Array(speakers) as _, speaker}
            <Speaker/>
        {/each}
        <button on:click={handleClick} class="add">+</button>
    </tbody>
</table>

