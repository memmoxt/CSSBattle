<div class="main">
    <svg viewBox="0 0 400 300">
        <mask id="half">
            <circle cx="50" cy="50" r="50" class="fill-[white] opacity-100"></circle>
            <circle cx="50" cy="50" r="30" class="fill-[black] opacity-100"></circle>
            <rect x="0" y="0" width="100" height="50" rx="0" ry="0" class="fill-[black]"></rect>
        </mask>

        <symbol id="orange-circle">
            <circle cx="50" cy="50" r="50" class="fill-[var(--orange)]"></circle>
        </symbol>
          
        <symbol id="complete-orange">
            <use xlink:href="#orange-circle" mask="url(#half)" x="0" y="0" width="" height="" class=""></use>
            <circle cx="10" cy="50" r="10" class="fill-[var(--orange)]"></circle>
        </symbol>

        <rect x="0" y="0" width="400" height="300" rx="0" ry="0" class="fill-[var(--beige)]"></rect>
        <use xlink:href="#complete-orange" x="70" y="100" width="" height="" class=""></use>
        <use xlink:href="#complete-orange" x="70" y="100" width="" height="" class="origin-center scale-x-[-1]"></use>
        <use xlink:href="#complete-orange" x="150" y="100" width="" height="" class="origin-center scale-y-[-1]"></use>
    </svg>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
        --beige:#f5d6b4;
        --orange:#d86f45;
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
	}
</style>

