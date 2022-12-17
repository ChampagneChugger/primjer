<script lang="ts">
    import "../style.css"
    import { scale } from "svelte/transition"
    import { page } from "$app/stores"
</script>
{#key $page}
<div in:scale class="container">
    <slot/>
</div>
{/key}