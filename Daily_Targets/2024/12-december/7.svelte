<div class="main">
	<div>
		<div></div>
	</div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--white: #ffffff;
		--green: #63a3a0;
		--dark: #0b2429;
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
			top: 0px;
			height: 150px;
			width: 400px;
        background-color:var(--green);
			/* opacity: 0.5; */
			& > div {
				bottom: -40px;
				left: 160px;
				position: absolute;
				height: 80px;
				border-radius: 50%;
				aspect-ratio: 1;
				background-color: var(--white);
                box-shadow:0 0 0 60px var(--dark);
			}
		}
	}
</style>

