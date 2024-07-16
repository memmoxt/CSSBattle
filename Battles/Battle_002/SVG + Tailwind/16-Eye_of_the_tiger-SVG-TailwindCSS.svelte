<div class="main">
    <svg viewBox="0 0 400 300">
        <!-- <rect x="0" y="0" width="100" height="100" rx="0" ry="0" class="fill-[red] translate-x-[129.5px] translate-y-[79.5px] opacity-50 rotate-45"></rect> -->
        <symbol id="rotated-square">
            <rect x="0" y="0" width="100" height="100" rx="0" ry="0" class="translate-x-[105px] translate-y-[0px] rotate-45"></rect>
        </symbol>

        <mask id="eye-mask">
            <use xlink:href="#rotated-square" x="0" y="0" width="" height="" class="fill-white 
                translate-x-[24.4px]
                translate-y-[79.3px]"></use>
            <use xlink:href="#rotated-square" x="0" y="0" width="" height="" class="fill-white 
                translate-x-[165.4px]
                translate-y-[79.3px]"></use>
            <circle cx="200" cy="150" r="100" class="fill-white"></circle>
            <circle cx="200" cy="150" r="90" class="fill-black"></circle>
            <circle cx="200" cy="150" r="70" class="fill-white"></circle>
            <circle cx="200" cy="150" r="25" class="fill-black"></circle>
        </mask>

        <rect  x="0" y="0" width="400" height="300" rx="0" ry="0" class="fill-[var(--green)]"></rect>
        <rect mask="url(#eye-mask)" x="0" y="0" width="400" height="300" rx="0" ry="0" class="fill-[var(--gold)]"></rect>
        <circle mask="url(#eye-mask)" cx="200" cy="150" r="70" class="fill-[var(--yellow)]"></circle>
    </svg>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
        --green:#0b2429;
        --gold:#998235;
        --yellow:#f3ac3c;
	}
	.main {
		height: 300px;
		width: 400px;
		display: grid;
	}
</style>

