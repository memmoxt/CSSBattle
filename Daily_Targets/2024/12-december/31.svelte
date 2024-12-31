<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--yellow: #fade8b;
		--blue: #328fc1;
        background-color:var(--blue);
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
			left: 0px;
            top: 0px;
			height: 275px;
            width: 150px;
			border-bottom-left-radius: 100px;
			border-bottom-right-radius: 100px;
            box-shadow:250px 0 0 var(--yellow);
			background-color: var(--yellow);
		}
	}
</style>

