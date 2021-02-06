<script>
    import CountButton from './CountButton.svelte';

    let speaker = {
        name: "",
        ah: 0,
        um: 0,
        er: 0,
        well: 0,
        so: 0,
        like: 0,
        but: 0,
        repeats: 0,
        other: 0
    }
</script>

<style>
    input {
        width: 200px;
    }

    .countbtn {
        width: 75px;
    }

</style>
<tr>
    <td><input type="text" bind:value={speaker.name} placeholder="John Doe"></td>
    <td class="countbtn"><CountButton value={speaker.ah}/></td>
    <td class="countbtn"><CountButton value={speaker.um}/></td>
    <td class="countbtn"><CountButton value={speaker.er}/></td>
    <td class="countbtn"><CountButton value={speaker.well}/></td>
    <td class="countbtn"><CountButton value={speaker.so}/></td>
    <td class="countbtn"><CountButton value={speaker.like}/></td>
    <td class="countbtn"><CountButton value={speaker.but}/></td>
    <td class="countbtn"><CountButton value={speaker.repeats}/></td>
    <td class="countbtn"><CountButton value={speaker.other}/></td>
</tr>