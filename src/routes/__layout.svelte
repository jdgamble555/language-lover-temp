<svelte:head>
	<meta name="description" content="A website with links on language learning, and language resources!">
</svelte:head>
<script type="ts">
	import { Navbar, Card } from 'spaper';
	import 'papercss/dist/paper.min.css';
</script>

<nav>
	<Navbar>
		<h3 slot="brand">
			<a href="/"><span class="color-red">❤</span> Language Lover</a>
		</h3>
		<ul class="inline">
			<li><a href="/">Login</a></li>
		</ul>
	</Navbar>
</nav>
<div class="s-container">
	<Card>
		<slot />
	</Card>
</div>

<style>
	.s-container {
		margin-top: 15px;
		margin-bottom: 15px;
		max-width: 995px;
        width: 100%;
		background-color: transparent !important;
		position: absolute;
		left: 50%;
		transform: translateX(-50%);
	}
    .color-red {
        color: rgb(150, 2, 2);
    }
</style>
