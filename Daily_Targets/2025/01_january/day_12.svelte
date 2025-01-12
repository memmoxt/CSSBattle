<div class="main">
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
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
		--green: #668884;
		--white: #eed9d9;
        background-color:var(--green);
		& > div {
			position: absolute;
			padding: 30px;
			height: 240px;
			width: 340px;
			background-color: var(--white);
			clip-path: polygon(
				0 0,
				21px 0px,
				21px 40px,
				34px 40px,
				34px 80px,
				55px 80px,
				55px 120px,
				89px 120px,
				89px 160px,
				144px 160px,
				144px 200px,
				233px 200px,
				233px 240px,
				0px 240px
			);
		}
		& > div:nth-child(2) {
			transform: scale(-1);
		}
	}
</style>

