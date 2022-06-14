<script>
import DirectionButton from "./_DirectionButton.svelte";
export let isFirstPicture;
    
</script>

<DirectionButton disabled={isFirstPicture} on:click>
    Left {isFirstPicture}
</DirectionButton>