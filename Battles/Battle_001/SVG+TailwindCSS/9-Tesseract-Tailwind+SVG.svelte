<div class="main">
	<svg viewBox="0 0 400 300">
		<rect x="0" y="0" height="300" width="400" rx="0" ry="0" class="fill-[var(--gray)]"></rect>
		<rect x="0" y="75" width="400" height="150" rx="0" ry="0" class="fill-[var(--blue)]"></rect>
        <rect x="75" y="25" height="250" width="250" rx="0" ry="0" class="origin-center rotate-45 fill-[var(--gray)]"></rect>
		<rect x="125" y="75" height="150" width="150" rx="0" ry="0" class="origin-center rotate-45 fill-[var(--blue)]" ></rect>
        <circle cx="200" cy="150" r="25" class="fill-[var(--slate)]"></circle>
	</svg>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--gray: #222730;
		--blue: #4caab3;
		--slate: #393e46;
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
	}
</style>

