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
		--green: #5aed9c;
		--purple: #4b4d88;
        background-color:var(--green)
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		flex-wrap: wrap;
		position: absolute;
		overflow: hidden;
		column-gap: 60px;
		& > div {
			position: absolute;
			height: 80px;
			width: 80px;
			background-color: var(--purple);
			clip-path: polygon(0 0, 30px 0px, 30px 50px, 80px 50px, 80px 80px, 0px 80px);
		}
		& > div:nth-child(2) {
			top: 60px;
			left: 210px;
		}
		& > div:nth-child(3) {
			top: 160px;
			left: 110px;
		}
	}
</style>

