<script lang="ts">
	import RecordTable from "$lib/components/RecordTable/RecordTable.svelte";
	import {
		egyptRecords,
		englandRecords,
		europeRecords,
		italyRecords,
		liverpoolRecords,
	} from "$lib/data";
</script>

<div class="my-8">
	<RecordTable recordSet={englandRecords} />
	<RecordTable recordSet={europeRecords} />
	<RecordTable recordSet={liverpoolRecords} />
	<RecordTable recordSet={egyptRecords} />
	<RecordTable recordSet={italyRecords} />
</div>
