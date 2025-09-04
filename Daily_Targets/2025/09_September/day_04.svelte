<div class="main">
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--green: #51a495;
		--white: #ffffff;
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
			height: 100px;
			aspect-ratio: 1;
			background-color: var(--white);
			translate: 20px;
			transform: rotate(45deg);
			box-shadow: 63px -63px var(--white);
		}
		& > div:nth-child(2) {
			transform: rotate(135deg);
			translate: -110px -40px;
			box-shadow: 56px -56px var(--white);
		}
	}
</style>
