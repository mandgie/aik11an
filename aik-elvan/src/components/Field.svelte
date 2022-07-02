<script>
    import Player from './Player.svelte';
    export let fieldNr;
</script>

<div>
    Field number: {fieldNr}
</div>
<div class="field-container">
    <Player player={'Nordfeldt'} posX={20} posY={240}/>
    <Player player={'Lustig'} posX={160} posY={50}/>
    <Player player={'Milosevic'} posX={140} posY={200}/>
    <Player player={'Sotte'} posX={140} posY={300}/>
    <Player player={'Otieno'} posX={160} posY={420}/>
    <Player player={'Elbouzedi'} posX={360} posY={50}/>
    <Player player={'Hussein'} posX={340} posY={200}/>
    <Player player={'Larsson'} posX={340} posY={300}/>
    <Player player={'Ahmed'} posX={360} posY={420}/>
    <Player player={'Bahoui'} posX={540} posY={200}/>
    <Player player={'Stefanelli'} posX={580} posY={300}/>
</div>



<style>
	.field-container {
        position: relative;
		color: purple;
        /*background-color: rgb(239, 244, 171);*/
        border: yellow 5px solid;
        width: 60%;
        height: 70%;
        margin: auto;
		font-family: 'Comic Sans MS', cursive;
        box-shadow: rgba(0, 0, 0, 0.19) 0px 10px 20px, rgba(0, 0, 0, 0.23) 0px 6px 6px;
	}
</style>