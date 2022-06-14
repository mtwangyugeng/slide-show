<script>
    export let disabled = false;
</script>

<button on:click disabled={disabled}>
    <slot />
</button>

<style>
    button:disabled {
        background-color: red;
        cursor: initial;
    }
</style>