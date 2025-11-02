<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--blue: #243d83;
		--yellow: #f0cd48;
        background-color:var(--blue);
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
			height: 40px;
			width: 320px;
			background-color: var(--yellow);
			translate: 0px 80px;
			&:before {
				content: '';
				position: absolute;
				height: 160px;
				width: 30px;
				background-color: var(--yellow);
				box-shadow:
					115px 0 var(--yellow),
					230px 0 var(--yellow);
				translate: 30px -160px;
			}
			&:after {
				content: '';
				position: absolute;
				height: 40px;
				aspect-ratio: 1;
				background-color: var(--yellow);
				box-shadow:
					115px -120px var(--yellow),
					230px 0px var(--yellow);
				translate: 25px -40px;
			}
		}
	}
</style>
