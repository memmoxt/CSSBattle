<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		/* box-sizing: content-box; */
		box-sizing: border-box;
		--purple: #3a335a;
		--yellow: #fade8b;
        background-color:var(--purple);
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
			height: 160px;
			width: 70px;
			background-color: var(--yellow);
			translate: -45px 0px;
			box-shadow: 90px 0 var(--yellow);
			&:before {
				content: '';
				position: absolute;
				height: 60px;
				width: 20px;
				background-color: var(--yellow);
				translate: -20px 50px;
				box-shadow:
					-40px -1px var(--yellow),
					-80px 0px var(--yellow),
                    180px 0px var(--yellow),
                    220px 0 var(--yellow),
                    260px 0px var(--yellow);
			}
		}
	}
</style>
