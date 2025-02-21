<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--gray: #3f4869;
		--darkyellow: #9c8a39;
		--yellow: #fbe374;
        background-color:var(--gray);
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
		& > div {
			position: absolute;
			height: 150px;
			width: 240px;
			top: 200px;
			background-color: var(--darkyellow);
			&::before {
				content: '';
				position: absolute;
				left: -0px;
				top: -47px;
				border-radius: 50%;
				height: 100px;
				width: 240px;
				background-color: var(--yellow);
			}
			&::after {
				position: absolute;
				content: '';
				top: -40px;
				left: 30px;
				height: 60px;
				width: 180px;
				background-color: var(--gray);
				border-radius: 50%;
			}
		}
	}
</style>

