<div class="main">
	<svg width="400" height="300" viewBox="0 0 400 300">
		<symbol id="leaf">
			<path d="M 226,75 C 171,75 126,120 126,176 V 225 H 175 C 231,225 276,180 276,124 V 75 Z"
			></path>
		</symbol>
		<rect x="0" y="0" width="400" height="300" rx="0" ry="0" class="fill-[var(--darkgreen)]"></rect>
		<use
			xlink:href="#leaf"
			x="0"
			y="0"
			width=""
			height=""
			class="translate-x-[-51px] fill-[var(--green)]"
		></use>
		<use
			xlink:href="#leaf"
			x="0"
			y="0"
			width=""
			height=""
			class="translate-x-[-1px] fill-[var(--gold)]"
		></use>
		<use
			xlink:href="#leaf"
			x="0"
			y="0"
			width=""
			height=""
			class="translate-x-[50px] fill-[var(--yellow)]"
		></use>
	</svg>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--darkgreen: #0b2429;
		--green: #1a4341;
		--gold: #998235;
		--yellow: #f3ac3c;
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
	}
</style>
