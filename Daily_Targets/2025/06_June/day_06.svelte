<div class="main">
	<div>
		<div></div>
		<div></div>
		<div></div>
		<div></div>
		<div></div>
		<div></div>
		<div></div>
		<div></div>
		<div></div>
	</div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--blue: #2d3464;
		--red: #d95362;
		--white: #c0d6e7;
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		position: absolute;
		overflow: hidden;
        background-color:var(--blue);
		& > div {
			display: grid;
			height: 210px;
			aspect-ratio: 1;
			justify-items: center;
			align-items: center;
			grid-template-columns: repeat(3, 1fr);
			grid-template-rows: repeat(3, 1fr);
			& > div {
				height: 50px;
				aspect-ratio: 1;
				background-color: var(--red);
			}
			& > div:nth-child(odd) {
				border-radius: 50%;
				background-color: var(--white);
			}
			& > div:nth-child(4) {
				&:before {
					width: 200px;
					height: 50px;
					transform: translate(-150px);
					content: '';
					position: absolute;
					background-color: var(--red);
					box-shadow: 300px 0 0 var(--red);
				}
			}
		}
	}
</style>
