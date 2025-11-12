<div class="main">
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--green: #bde4c1;
		--red: #9f6766;
        background-color:var(--green) ;
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
			height: 70px;
			width: 196px;
			background-color: var(--red);
			&:before {
				content: '';
				position: absolute;
				height: 100px;
				width: 40px;
				background-color: var(--red);
				translate: -40px 69px;
			}
			&:after {
				content: '';
				position: absolute;
				height: 30px;
				aspect-ratio: 1;
				background-color: var(--red);
				translate: -86px 69px;
				box-shadow: 0px 70px var(--red);
			}
		}
		& > div:nth-child(1) {
			transform: scale(-1);
		}
	}
</style>
