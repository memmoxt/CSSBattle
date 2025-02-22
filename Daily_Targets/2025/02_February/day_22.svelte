<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--brown: #96551a;
		--orange: #ea9a52;
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
        background-color:var(--brown);
		& > div {
			height: 300px;
			width: 140px;
			background-color: var(--orange);
			&:before {
				content: '';
				position: absolute;
				left: 165px;
				top: 115px;
				height: 70px;
				width: 70px;
				background-color: var(--brown);
			}
			&:after {
				content: '';
				position: absolute;
				left:130px;
				top: 140px;
				height: 20px;
				width: 140px;
				background-color: var(--brown);
			}
		}
	}
</style>

