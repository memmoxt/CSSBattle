<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
	}

	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		overflow: hidden;
		position: absolute;
		flex-wrap: wrap;
		gap: 20px;
		--red: #de6b67;
		--yellow: #eddf5a;
		background-color: var(--red);
		& > div {
			position: absolute;
			height: 300px;
			width: 400px;
			background-color: var(--yellow);
			clip-path: polygon(
				0 214px,
				160px 214px,
				160px 94px,
				187px 94px,
				187px 20px,
				213px 20px,
				213px 94px,
				240px 94px,
				240px 214px,
				400px 214px,
				400px 240px,
				214px 240px,
				214px 150px,
				186px 150px,
				186px 240px,
				0px 240px
			);
		}
	}
</style>
