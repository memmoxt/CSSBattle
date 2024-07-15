<div class="main">
	<svg viewBox="0 0 400 300">
		<defs>
			<symbol id="mini">
				<circle cx="50" cy="50" r="30" class=""></circle>
			</symbol>
			<symbol id="max">
				<circle cx="50" cy="50" r="50" class=""></circle>
			</symbol>

			<symbol id="ball-1">
				<use xlink:href="#max" x="" y="" width="" height="" class="fill-[var(--red)]"></use>
				<use xlink:href="#mini" x="" y="" width="" height="" class="fill-[var(--amber)]"></use>
			</symbol>

			<symbol id="ball-2">
				<use xlink:href="#max" x="" y="" width="" height="" class="fill-[var(--amber)]"></use>
				<use xlink:href="#mini" x="" y="" width="" height="" class="fill-[var(--red)]"></use>
			</symbol>
		</defs>

		<rect x="0" y="0" width="400" height="300" rx="0" ry="0" class="fill-[var(--purple)]"></rect>
		<polygon
			points="50,300 50,200 150,200 150,100 250,100 250,200 350,200 350,300"
			class="fill-[var(--yellow)]"
		></polygon>

		<use xlink:href="#ball-1" x="50" y="150" width="" height="" class=""></use>
		<use xlink:href="#ball-2" x="150" y="50" width="" height="" class=""></use>
		<use xlink:href="#ball-1" x="250" y="150" width="" height="" class=""></use>
	</svg>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--purple: #62306d;
		--yellow: #f7ec7d;
		--red: #aa445f;
		--amber: #e38f66;
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
	}
</style>
