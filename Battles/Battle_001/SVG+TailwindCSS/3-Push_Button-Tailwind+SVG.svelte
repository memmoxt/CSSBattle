<div class="main">
	<div class="h-[150px] w-[300px]">
		<svg viewBox="0 0 100 100" class="">
			<symbol id="circle">
				<circle cx="50" cy="50" r="10" class=""></circle>
			</symbol>

			<rect x="0" y="0" width="100" height="50" rx="0" ry="0" class="fill-[var(--blue)]"></rect>
			<use
				xlink:href="#circle"
				x="0"
				y="-6.00"
				class="origin-center scale-[4.17] fill-[var(--cyan)] opacity-100"
			></use>
			<use
				xlink:href="#circle"
				x="0"
				y="-10"
				class="origin-center scale-[2.5] fill-[var(--blue)] opacity-100"
			></use>
			<use
				xlink:href="#circle"
				x="0"
				y="-30"
				class="origin-center scale-[0.83] border-2 border-solid border-red-500 fill-[var(--yellow)] opacity-100"
			></use>
		</svg>
	</div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--cyan: #6592cf;
		--blue: #243d83;
		--yellow: #eeb850;
	}
	.main {
		background-color: var(--cyan);
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
	}
</style>
