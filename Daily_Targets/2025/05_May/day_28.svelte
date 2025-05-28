<div class="main">
	<div></div>
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--blue: #6592cf;
		--orange: #eeb850;
        background-color:var(--blue);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		position: absolute;
		overflow: hidden;
		flex-direction: column;
		row-gap: 30px;

		& > div {
			height: 70px;
			width: 180px;
			background-color: var(--orange);
			&:before {
				content: '';
				position: absolute;
				height: 80px;
				width: 70px;
				background-color: var(--orange);
				transform: translate(0px, -5px);
				box-shadow: 110px 0 var(--orange);
			}
		}
		& > div:nth-child(odd) {
			&:before {
				transform: translate(55px, -5px);
				box-shadow: 0 0 transparent;
			}
		}
	}
</style>
