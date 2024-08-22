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
		--green: #bde4c1;
		--purple: #784972;
        background-color:var(--green);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		& > div:nth-child(1) {
			transform: translateY(14px);
			height: 214px;
			width: 104px;
			background-color: var(--purple);
			border-radius: 50%;
		}
		& > div:nth-child(2) {
			align-self: start;
			height: 110px;
			position: absolute;
			width: 200px;
			background-color: transparent;
			border-top: 100px solid var(--purple);
			border-right: 100px solid transparent;
			border-bottom: 100px solid transparent;
			border-left: 100px solid transparent;
		}
		& > div:nth-child(3) {
			align-self: end;
			height: 110px;
			position: absolute;
			background-color: transparent;
			border-top: 100px solid transparent;
			border-right: 100px solid transparent;
			border-bottom: 100px solid var(--purple);
			border-left: 100px solid transparent;
		}
	}
</style>

