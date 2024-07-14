<div class="main">
	<div class="h-[300px] w-[400px] overflow-hidden">
		<svg viewBox="0 0 100 100">
			{#each Array(9) as _, i}
				<line
					x1={10 * (i + 1)}
					y1="0"
					x2={10 * (i + 1)}
					y2="75"
					class="stroke-red-500 stroke-[0.1px]"
				></line>
				<line
					x1="0"
					y1={10 * (i + 1)}
					x2="100"
					y2={10 * (i + 1)}
					class="stroke-red-500 stroke-[0.1px]"
				></line>
			{/each}

			<symbol id="symbol">
				<circle cx="50" cy="37.5" r="15.05" class=" opacity-100"></circle>
				<rect x="50" y="22.5" width="15" height="14.5" rx="0" ry="0" class="opacity-100"></rect>
			</symbol>

			<rect x="0" y="0" width="100" height="100" rx="0" ry="0" class="fill-[var(--green)]"></rect>
			<use
				xlink:href="#symbol"
				x="-15"
				y="40"
				width=""
				height=""
				class="origin-center rotate-180 fill-[var(--yellow)]"
			></use>
			<use xlink:href="#symbol" x="0" y="0" width="" height="" class="fill-[var(--neutral)]"></use>
			<use xlink:href="#symbol" x="-15" y="15" width="" height="" class="fill-[var(--yellow)]"
			></use>
		</svg>
	</div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--green: #0b2429;
		--yellow: #f3ac3c;
		--neutral: #998235;
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
	}
</style>
