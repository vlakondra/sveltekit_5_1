<script>
	import '../app.css';
	let { children } = $props();
	let p = $state(99);
</script>

<h1>test</h1>
<div class="first">
	{@render children()}
</div>

<style>
	.first {
		border: 1px solid silver;
		margin: 10px;
		padding: 10px;
	}
</style>
