<div class="main">
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--blue: #5dbcf9;
		--yellow: #ffffcd;
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
			height: 180px;
			width: 145px;
			/* opacity: 0.4; */
			translate: -70px;
			overflow: hidden;
			&:before {
				content: '';
				position: absolute;
				height: 300px;
				aspect-ratio: 1;
				background-color: var(--blue);
				border-radius: 50%;
				translate: 52px -60px;
				box-shadow: 0 0 0 50px var(--yellow);
			}
			&:after {
				content: '';
				position: absolute;
				height: 180px;
				width: 35px;
				background-color: var(--yellow);
				/* background-color:black;  */
				translate: 118px;
			}
		}
		& > div:nth-child(2) {
			transform: translate(140px) scale(-1);
		}
	}
</style>
