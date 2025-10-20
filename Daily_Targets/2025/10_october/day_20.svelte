<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--pink: #d8bec4;
		--red: #a34d60;
        background-color: var(--pink);
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
			height: 140px;
			width: 80px;
            translate: 40px;
			background-color: var(--red);
            border-top-right-radius: 80px;
            border-top-left-radius: 0px;
            border-bottom-right-radius: 0px;
            border-bottom-left-radius: 80px;
            box-shadow: -40px 0px var(--pink), -80px 0px var(--red);
		}
	}
</style>
