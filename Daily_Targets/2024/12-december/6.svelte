<div class="main">
	<div></div>
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--yellow: #f3ac3c;
        --green:#0b2429;
        background-color:var(--green);
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
			height: 60px;
			width: 180px;
			background-color: var(--yellow);
		}
		& > div:nth-child(1) {
			border-top-left-radius: 60px;
			border-bottom-right-radius: 60px;
		}
		& > div:nth-child(2) {
			top: 60px;
			border-top-left-radius: 60px;
			border-top-right-radius: 60px;
		}
		& > div:nth-child(3) {
			top: 180px;
		}
	}
</style>
