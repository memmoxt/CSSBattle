<div class="main">
	<div><div></div></div>
	<div><div></div></div>
	<div><div></div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--yellow: #f2eaa8;
		--purple: #7e6293;
		--red: #de6b67;
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
			position: absolute;
			aspect-ratio: 1;
			background-color: red;
			border-radius: 50%;
			overflow: hidden;
			& > div {
				background-color: var(--purple);
				height: 25px;
				width: 50px;
				box-shadow: 0 25px 0 0 var(--red);
			}
		}
		& > div:nth-child(1) {
			right: 25px;
		}
		& > div:nth-child(2) {
			right: 100px;
			transform: scale(-2);
		}
		& > div:nth-child(3) {
			right: 250px;
			transform: scale(4);
		}
	}
</style>

