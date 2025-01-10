<div class="main">
	<div><div></div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
	}

	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		overflow: hidden;
		position: absolute;
		flex-wrap: wrap;
		gap: 20px;
		--white: #ffe4e0;
		--red: #e05947;
        background-color:var(--white);
		& > div {
			position: absolute;
			height: 250px;
			width: 300px;
            clip-path: polygon(0px 85px,100px 85px,100px 40px,194px 40px,195px 85px, 300px 85px, 300px 250px,0px 250px);
			overflow: hidden;
			& > div {
				position: absolute;
				top: -15px;
				left: 50px;
				height: 200px;
				aspect-ratio: 1;
				background-color: var(--white);
				border-radius: 50%;
				box-shadow: 0 0 0 50px var(--red);
				&:before {
					content: '';
					position: absolute;
					left: 75px;
					top: 80px;
					height: 140px;
					width: 50px;
					background-color: var(--red);
				}
			}
		}
	}
</style>

