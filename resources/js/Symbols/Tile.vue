<script setup lang="ts">
const props = defineProps(['id'])
</script>
<template>
	<div id="tile-{{id}}" class="tile">
		<span class="tile-id">{{id}}</span>
		<slot/>
	</div>
</template>
