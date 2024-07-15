<div class="main">
    <svg viewBox="0 0 400 300">
        <symbol id="triangle">
            <polygon points="0,0 75,130 150,0" class=""></polygon>
        </symbol>

        <rect x="0" y="0" width="400" height="300" rx="0" ry="0" class="fill-[var(--yellow)]"></rect>

        <use xlink:href="#triangle" x="0" y="0" width="" height="" class="translate-x-[80px] translate-y-[85px] fill-[var(--red)]"></use>
        <use xlink:href="#triangle" x="0" y="0" width="" height="" class="translate-x-[60px] translate-y-[85px] fill-[var(--orange)]"></use>

        <use xlink:href="#triangle" x="0" y="0" width="" height="" class="translate-x-[340px] translate-y-[215px] fill-[var(--orange)] rotate-180"></use>
        <use xlink:href="#triangle" x="0" y="0" width="" height="" class="translate-x-[320px] translate-y-[215px] fill-[var(--red)] rotate-180"></use>
    </svg>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--yellow: #f2f2b6;
        --orange:#ff6d00;
        --red:#fd4602;
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
	}
</style>

