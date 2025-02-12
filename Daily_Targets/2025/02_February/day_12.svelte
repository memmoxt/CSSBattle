<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--black: #343d42;
		--purple: #7c87d1;
        background-color:var(--black);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		position: absolute;
		overflow: hidden;
		& > div {
			position: absolute;
			top: 40px;
			height: 220px;
			width: 220px;
			border-radius: 50%;
			background-color: var(--purple);
			/* opacity: 0.5; */
			clip-path: polygon(0 0, 220px 0px, 220px 170px, 0px 170px);

			&:before {
				content: '';
				position: absolute;
				top: 130px;
				height: 100px;
				width: 220px;
				background-color: var(--purple);
				box-shadow: 0 -20px var(--black);
			}
			&:after {
				content: '';
				position: absolute;
				top: 35px;
                left:90px;
				height: 90px;
				width: 40px;
				background-color: var(--black);
			}
		}
	}
</style>

