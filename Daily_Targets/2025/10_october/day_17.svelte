<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--blue: #243d83;
		--orange: #e8ad6d;
        background-color: var(--blue);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		overflow: hidden;
		position: absolute;
		& > div {
			position: absolute;
			height: 20px;
			width: 250px;
			background-color: var(--orange);
			translate: -10px -20px;
			box-shadow:
				0px 40px var(--orange),
				20px 40px var(--orange);
			&:before {
				content: '';
				position: absolute;
				height: 106px;
				aspect-ratio: 1;
				background-color: var(--orange);
				border-radius: 50%;
				box-shadow: 118px 0px var(--orange);
				translate: 45px -24px;
				clip-path: polygon(0px 0px, 250px 0px, 250px 44px, 0px 44px);
			}
		}
	}
</style>
