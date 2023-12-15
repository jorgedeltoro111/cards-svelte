<script>
    export let data;
    let band = false;
    let messageButton = 'Ver mensaje';
    function showMessage(){
        band = !band;
        if(band){
            messageButton = 'Cerrar';
        }else{
            messageButton = 'Ver mensaje';
        }

    }
</script>

<style>
    .Card-content{
        border: 2px solid black;
        background-color: white;
        flex: 1;
        border-radius: 10px;
        text-align: center;
        margin-left: 25%;
        margin-right: 25%;
    }
    button{
        border-radius: 10px;
    }
    .Card-container{
        margin: 5px;
    }
    p{
        text-align: justify;
        margin: 5px;
    }
</style>

<div class="Card">
    <div class="Card-container">
        <div class="Card-content">
            <h1>{data.title}</h1>
            <div class="Card-message">
                {#if band}
                    <p>{data.message}</p>
                {/if}
            </div>
            <button on:click={showMessage}>{messageButton}</button>
        </div>
    </div>
</div>