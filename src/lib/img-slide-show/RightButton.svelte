<script>
    import DirectionButton from "./_DirectionButton.svelte";
    export let isLastPicture;
        
</script>

<DirectionButton disabled={isLastPicture} on:click>
    right {isLastPicture}
</DirectionButton>