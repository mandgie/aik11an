<script>

    function handleMouseOut(nr) {
        if (!starChecked) {
            for (let key in star_state) {
                if (key <= nr) {
                    star_state[key] = false
                }
            }
        }
    }

    function handleMouseOver(nr) {
        if (!starChecked) {
            for (let key in star_state) {
                if (key <= nr) {
                    star_state[key] = true
                }
            }
        }
    }

    function handleClick(nr) {
        if (!starChecked) {
            for (let key in star_state) {
                if (key <= nr) {
                    star_state[key] = true
                }
            }
        }
        starChecked = true;
    }

    const star_state = {
        '1': false,
        '2': false,
        '3': false,
        '4': false,
        '5': false
    };

    let starChecked = false;

</script>

<div>
    <span class="fa fa-star star" style="color: {(star_state['1'] ? 'yellow' : 'black')}" on:click={() => handleClick(1)} on:mouseover={() => handleMouseOver(1)} on:mouseout={() => handleMouseOut(1)}></span>
    <span class="fa fa-star star" style="color: {(star_state['2'] ? 'yellow' : 'black')}" on:click={() => handleClick(2)} on:mouseover={() => handleMouseOver(2)} on:mouseout={() => handleMouseOut(2)}></span>
    <span class="fa fa-star star" style="color: {(star_state['3'] ? 'yellow' : 'black')}" on:click={() => handleClick(3)} on:mouseover={() => handleMouseOver(3)} on:mouseout={() => handleMouseOut(3)}></span>
    <span class="fa fa-star star" style="color: {(star_state['4'] ? 'yellow' : 'black')}" on:click={() => handleClick(4)} on:mouseover={() => handleMouseOver(4)} on:mouseout={() => handleMouseOut(4)}></span>
    <span class="fa fa-star star" style="color: {(star_state['5'] ? 'yellow' : 'black')}" on:click={() => handleClick(5)} on:mouseover={() => handleMouseOver(5)} on:mouseout={() => handleMouseOut(5)}></span>
</div>


<style>
    .star {
        color: black;
        margin: 0px;
        padding: 0px;
        font-size: 15px;
    }

    .checked-star {
        color: blue;
    }
/*
    .star:hover {
        color: yellow;
    }
*/
</style>