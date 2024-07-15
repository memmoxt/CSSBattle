<div class="main">
	<svg viewBox="0 0 400 300">
		<mask id="small-circle-mask">
			<rect x="0" y="0" width="100" height="50" rx="0" ry="0" class="fill-white"></rect>
			<circle cx="50" cy="50" r="30" class="fill-black"></circle>
		</mask>

        <mask id="big-circle-mask">
            <circle cx="70" cy="70" r="70" class="fill-white"></circle>
            <circle cx="70" cy="70" r="50" class="fill-black"></circle>
        </mask>

		<symbol id="mini" viewBox="0 0 400 300"
			><circle cx="50" cy="50" r="50" mask="url( #small-circle-mask )" class="fill-[var(--yellow)]"
			></circle>
        </symbol>


        <rect x="0" y="0" width="400" height="300" rx="0" ry="0" class="fill-[var(--brown)]"></rect>
        <use xlink:href="#mini" x="0" y="0" width="" height="" class="translate-x-[-250px] translate-y-[-100px] origin-center rotate-180"></use>
        <use xlink:href="#mini" x="0" y="0" width="" height="" class="translate-x-[250px] translate-y-[100px] origin-center"></use>
        <circle cx="70" cy="70" r="70" mask="url(#big-circle-mask)" class="fill-[var(--yellow)] translate-x-[130px] translate-y-[80px]"></circle>
        <circle cx="50" cy="50" r="25" class="fill-[var(--red)] translate-x-[150px] translate-y-[100px]"></circle>
	</svg>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--brown: #191210;
		--yellow: #eca03d;
		--red: #84271c;
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
	}
</style>

