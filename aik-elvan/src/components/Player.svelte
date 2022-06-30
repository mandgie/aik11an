<script>

    import Stars from './Stars.svelte'
    export let player;
    export let posX;
    export let posY;

    function handleMouseOut(e) {
        console.log('sadf');
    }

    function handleMouseOver(e) {
        const stars = document.querySelectorAll('.star');
        console.log(stars);
    }
</script>



<div class="player" style="top: {posX + 'px'}; left: {posY + 'px'}">
        <div class="player-style">{player}</div>
        <Stars />
</div>





<style>
    .player {
        color: yellow;
        position: absolute;
        top: 140px;
        left:120px;
        box-shadow: rgba(0, 0, 0, 0.12) 0px 1px 3px, rgba(0, 0, 0, 0.24) 0px 1px 2px;
    }
    .player-style {
        background-color: black;
        font-size: 30px;
    }

    .star {
        color: black;
    }

    .star:hover {
        color: yellow;
    }
</style>