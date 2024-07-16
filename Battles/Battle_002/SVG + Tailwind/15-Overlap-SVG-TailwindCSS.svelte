<div class="main">
	<svg viewBox="0 0 400 300">
		<mask id="lua">
			<circle cx="75" cy="75" r="75" class="translate-x-[0px] translate-y-[0px] fill-[white]"
			></circle>
			<circle cx="75" cy="75" r="75" class="translate-x-[100px] translate-y-[0px] fill-[black]"
			></circle>
		</mask>

        <symbol id="half-shape">
            <circle cx="75" cy="75" r="75" mask="url(#lua)" class=""></circle>
        </symbol>

        <rect x="0" y="0" width="400" height="300" rx="0" ry="0" class="fill-[var(--blue)]"></rect>
        <use xlink:href="#half-shape" x="0" y="0" width="" height="" class=" translate-x-[75px] translate-y-[75px] fill-[var(--purple)]"></use>
        <use xlink:href="#half-shape" x="0" y="0" width="" height="" class="rotate-180 translate-x-[325px] translate-y-[225px] fill-[var(--pink)]"></use>
	</svg>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--blue: #09042a;
		--purple: #7b3f61;
		--pink: #e78481;
	}
	.main {
		height: 300px;
		width: 400px;
		display: grid;
	}
</style>

