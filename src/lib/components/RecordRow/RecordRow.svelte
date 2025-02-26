<script lang="ts">
	import type { Record } from "$lib/data";

	interface Props {
		record: Record;
	}

	let { record }: Props = $props();
</script>

<div class="border-b border-white/30 px-4 py-2 first:border-t lg:px-6 lg:py-4">
	<p class="font-display mb-2 text-xl lg:text-2xl">{record.description}</p>
	{#if record.info}
		<p class="text-sm lg:text-base">({record.info})</p>
	{/if}
</div>
