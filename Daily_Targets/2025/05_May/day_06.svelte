<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--white: #ebf6f0;
		--brown: #4e4b44;
		--green: #4a9a86;
        background-color:var(--white);
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
			position: abstolute;
			height: 70px;
			width: 400px;
			background-color: var(--brown);
			transform: translate(0px, 117px);
			&:before {
				content: '';
				position: absolute;
				height: 40px;
				aspect-ratio: 1;
				background-color: var(--green);
				border-radius: 50%;
				transform: translate(35px, -20px);
				box-shadow:
					63px 0px 0 10px var(--green),
					145px 0 0 20px var(--green),
					226px 0 0 10px var(--green),
					289px 0 var(--green);
			}
		}
	}
</style>
