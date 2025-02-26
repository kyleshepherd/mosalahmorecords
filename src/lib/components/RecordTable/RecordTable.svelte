<script lang="ts">
	import type { RecordSet } from "$lib/data";
	import RecordRow from "../RecordRow/RecordRow.svelte";

	interface Props {
		recordSet: RecordSet;
	}

	let { recordSet }: Props = $props();
</script>

<div class="mx-auto mt-6 max-w-[1280px] px-4 first:mt-0">
	<h2 class="font-display px-4 py-2 text-4xl lg:px-6 lg:py-4 lg:text-5xl">{recordSet.name}</h2>
	<div>
		{#each recordSet.records as record}
			<RecordRow {record} />
		{/each}
	</div>
</div>
