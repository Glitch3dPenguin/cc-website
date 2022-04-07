<script>
	import { onMount } from 'svelte';

	export let redirectLink;

	onMount(() => {
		location.replace(redirectLink);
	});
</script>

<div
	class="container"
	style="display: flex; justify-content: center; align-items: center; margin-top: 3.5em;"
>
	<div class="has-text-centered">
		<a id="redirect" href={redirectLink}> Click here if you are not redirected </a>
	</div>
</div>
