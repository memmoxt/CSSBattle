<div class="main">
	<div>
		<div></div>
		<div></div>
		<div></div>
		<div></div>
		<div></div>
		<div></div>
		<div></div>
		<div></div>
		<div></div>
		<div></div>
		<div></div>
		<div></div>
	</div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--purple: #7e6293;
		--yellow: #ebe77e;
		--orange: #de817e;
        background-color: var(--purple);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		overflow: hidden;
		position: absolute;
		& > div:nth-child(1) {
			height: 220px;
			width: 320px;
			display: grid;
			gap: 20px 40px;
			grid-template-columns: repeat(3, 1fr);
			grid-template-rows: repeat(4, 1fr);
			& > div {
				position: relative;
				height: 40px;
				aspect-ratio: 1;
				border-radius: 50%;
				background-color: var(--orange);
				justify-self: center;
			}
		}
		& > div:nth-child(2) {
			position: absolute;
			height: 220px;
			width: 40px;
			translate: -60px;
			background-color: var(--yellow);
			box-shadow: 120px 0px var(--yellow);
		}
	}
</style>
