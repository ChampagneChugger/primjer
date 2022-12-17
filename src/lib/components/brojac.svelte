<script lang="ts">
    let number: number = 0

    $: positive = number > 0
    $: negative = number < 0
</script>

<div class="brojac">
    <button on:click={() => number--}>-</button>
    <p class:positive class:negative>{number}</p>
    <button on:click={() => number++}>+</button>
</div>
<a class="natrag" href="./">Idi unatrag</a>