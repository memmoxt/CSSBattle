<script lang="ts">
	import cssbattle from '$lib/images/today.png';
	import CSS_Battle from './CSS_Battle.svelte';
</script>

<div class="flex flex-col items-center justify-between">
	<div style="height:300px;width:400px;" class="m-4 box-border">
		<img
			src={cssbattle}
			alt="cssbattle"
			class="cssbattle-image absolute"
			style="opacity:0.5;height:300px;width:400px; z-index:-10;"
		/>
		<div class="height[300px] width[400px] absolute" style="z-index:-9;">
			<!-- NOTE: CSSBattle -->
			<CSS_Battle />
		</div>
	</div>
	<img src={cssbattle} alt="cssbattle" class=" m-4" style="height:300px;width:400px;" />
</div>
