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

			<defs>
				<mask id="circleMask">
					<circle cx="50" cy="37.5" r="25" class="fill-white"></circle>
				</mask>
			</defs>

			<symbol id="rects">
				<rect width="25" height="25" rx="0" ry="0" class=""></rect>
			</symbol>

			<rect x="0" y="0" width="100" height="75" rx="0" ry="0" class="fill-[var(--red)]"></rect>
			<g mask="url(#circleMask)">
				<use xlink:href="#rects" x="25" y="12.5" width="" height="" class="fill-[var(--teal)]"
				></use>
				<use xlink:href="#rects" x="50" y="12.5" width="" height="" class="fill-[var(--yellow)]"
				></use>
				<use xlink:href="#rects" x="25" y="37.5" width="" height="" class="fill-[var(--white)]"
				></use>
			</g>
		</svg>
	</div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--teal: #51b5a9;
		--red: #e3516e;
		--white: #f7f3d7;
		--yellow: #fade8b;
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
	}
</style>
