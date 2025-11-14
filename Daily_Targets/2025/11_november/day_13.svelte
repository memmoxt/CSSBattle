
<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--green: #264629;
		--yellow: #f8b140;
		--red: #cf6939;
        background-color: var(--green);
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
			height: 140px;
			aspect-ratio: 1;
			background-color: var(--red);
			box-shadow: 0 0 0 40px var(--yellow);
			&:before,
			&:after {
				content: '';
				position: absolute;
				height: 20px;
				width: 80px;
				translate: -40px 60px;
				box-shadow: 140px 0px var(--green);
				background-color: var(--green);
			}
			&:after {
				transform: rotate(90deg) translate(-70px, -70px);
			}
		}
	}
</style>
