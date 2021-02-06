<script>
export let value = 0;

function handleClick(){
    value += 1;
}

</script>

<style>
/* take 100% of the available space defined by parent DOM-element */
button{
    width: 100%;
}
</style>


<button on:click={handleClick}>{value}</button>