<div class="main">
	<div class="pizza"></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		background-color: #e3516e;
	}

	.main {
		height: 100vh;
		display: flex;
		justify-content: center;
		align-items: center;

		& .pizza {
			border-radius: 50%;
			border-top: 100px solid #51b5a9;
			border-right: 100px solid #fade8b;
			border-left: 100px solid #f7f3d7;
			border-bottom: 100px solid transparent;
			transform: rotate(-45deg);
		}
	}
</style>
