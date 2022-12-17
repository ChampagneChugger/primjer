<script lang="ts">
    export let ime: string = ""
</script>
<div class="unosc">
    {#if ime == ""}
    <p>Pozdrav, nepoznati.</p>
    {:else}
        <p>Pozdrav, {ime}.</p>
    {/if}
    <input placeholder="Vaše ime" bind:value={ime}>
</div>