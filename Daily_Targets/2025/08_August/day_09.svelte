<div class="main">
	<div><div></div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		/* box-sizing: content-box; */
		box-sizing: border-box;
		--yellow: #fade8b;
		--lightgreen: #31938c;
		--darkgreen: #135853;
        background-color:var(--yellow);
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
			overflow: hidden;
			position: absolute;
			height: 250px;
			width: 300px;
			& > div {
				height: 250px;
				width: 140px;
				background-color: var(--lightgreen);
				translate: 30px 0px;
				border-top-right-radius: 70px;
				border-top-left-radius: 70px;
				box-shadow:
					100px 0 var(--lightgreen),
					-100px 0 var(--lightgreen);

				&:before {
					content: '';
					position: absolute;
					height: 30px;
					width: 240px;
					background-color: var(--darkgreen);
					translate: 0 220px;
				}
				&:after {
					content: '';
					position: absolute;
					height: 210px;
					width: 60px;
					background-color: var(--yellow);
					border-top-right-radius: 50px;
					border-top-left-radius: 50px;
					translate: 40px 40px;
					box-shadow:
						100px 0px var(--yellow),
						-100px 0px var(--yellow);
				}
			}
		}
	}
</style>
