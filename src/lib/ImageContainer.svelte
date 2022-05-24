<script>
    export let title = "<Enter Title>";
    export let url = "";
    export let description = "<Enter Description>"

    export let width = 400;
    export let height = 400;
</script>

<div>
    <section style={`width: ${width}px; height: ${height}px`}>
        <div class=Background style={`background-image: url(${url})`}/>
        <img src={url} alt={title} />
    </section>
    <p>{description}</p>
</div>

<style>
    section {
        display: flex;
        justify-content: center;
        align-items: center;

        position: relative;


    }



    .Background {
        position: absolute;
        width: 100%;
        height: 100%;
        filter: blur(7px);
        
        background-position: center;
        background-repeat: no-repeat;
        background-size: cover;
        z-index: 1;
    }

    img {
        z-index: 2;
    }
</style>
