<script>
    import Player from './Player.svelte';
    export let fieldNr;
</script>

<div>
    Field number: {fieldNr}
</div>
<div class="field-container">
    <Player player={'PK'} posX={20} posY={250}/>
    <Player player={'PK'} posX={160} posY={50}/>
    <Player player={'AM'} posX={140} posY={200}/>
    <Player player={'SS'} posX={140} posY={300}/>
    <Player player={'PK'} posX={160} posY={400}/>
    <Player player={'PK'} posX={360} posY={80}/>
    <Player player={'AM'} posX={340} posY={200}/>
    <Player player={'SS'} posX={340} posY={300}/>
    <Player player={'PK'} posX={360} posY={420}/>
    <Player player={'SS'} posX={540} posY={200}/>
    <Player player={'PK'} posX={580} posY={300}/>
</div>



<style>
	.field-container {
        position: relative;
		color: purple;
        background-color: lightgreen;
        width: 60%;
        height: 70%;
        margin: auto;
		font-family: 'Comic Sans MS', cursive;
        box-shadow: rgba(0, 0, 0, 0.19) 0px 10px 20px, rgba(0, 0, 0, 0.23) 0px 6px 6px;
	}
</style>