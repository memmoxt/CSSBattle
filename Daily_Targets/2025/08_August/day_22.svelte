<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--white: #ffffff;
		--red: #f88889;
		--black: #000000;
        background-color:var(--white);
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
			height: 300px;
			width: 50px;
			background-color: var(--red);
			translate: -95px 0px;
			box-shadow: 190px 0px var(--red);
			&:before {
				content: '';
				position: absolute;
				height: 50px;
				aspect-ratio: 1;
				background-color: var(--black);
				border-radius: 50%;
				translate: -30px 125px;
				box-shadow: 250px 0 var(--black);
			}
			&:after {
				content: '';
				position: absolute;
				height: 50px;
				width: 255px;
				background-color: var(--black);
				translate: -7px 125px;
			}
		}
	}
</style>
