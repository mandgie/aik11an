<script>
    import Field from '../components/FieldContainer.svelte';
    import Header from '../components/Header.svelte';
</script>

<div>
    <div class="container">
        <Header />
        <Field />
    </div>
</div>

<style>
	.container {
        width: 920px;
        height: 1000px;
		margin: auto;
		font-family: 'Comic Sans MS', cursive;
        text-align: center;
	}
    :global(body) {
		background-color: #49494f;
	}
</style>
