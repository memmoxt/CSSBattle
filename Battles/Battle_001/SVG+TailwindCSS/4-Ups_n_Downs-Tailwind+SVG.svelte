<div class="main">
	<div class="h-[300px] w-[400px]">
		<svg viewBox="0 0 100 100">
			{#each Array(9) as _, i}
				<line
					x1={10 * (i + 1)}
					y1="0"
					x2={10 * (i + 1)}
					y2="75"
					class="stroke-indigo-500 stroke-[0.1px]"
				></line>
				<line
					x1="0"
					y1={10 * (i + 1)}
					x2="100"
					y2={10 * (i + 1)}
					class="stroke-indigo-500 stroke-[0.1px]"
				></line>
			{/each}
			<symbol id="is">
				<rect x="12.5" y="37.5" rx="0" ry="0" width="25" height="12" class="fill-[var(--yellow)]"
				></rect>
				<rect x="12.5" y="37.5" rx="50" ry="50" width="25" height="25" class="fill-[var(--yellow)]"
				></rect>
			</symbol>

			<rect x="0" y="0" rx="0" ry="0" width="100" height="75" class="fill-[var(--purple)]"></rect>
			<use xlink:href="#is" x="0" y="0" class=""></use>
			<use xlink:href="#is" x="50" y="0" class=""></use>
			<use xlink:href="#is" x="25" y="25" class="origin-center scale-y-[-1]"></use>
		</svg>
	</div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--yellow: #f7ec7d;
		--purple: #62306d;
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
	}
</style>
