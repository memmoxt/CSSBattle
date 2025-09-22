<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--white: #fef6e2;
		--blue: #161e44;
        background-color:var(--white);
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
			height: 50px;
			width: 270px;
			translate: 0px -35px;
			background-color: var(--blue);
			&:before {
				content: '';
				position: absolute;
				height: 50px;
				width: 200px;
				background-color: var(--blue);
				translate: 35px 90px;
			}
			&:after {
				content: '';
				position: absolute;
				height: 220px;
				width: 30px;
				background-color: var(--blue);
				translate: 120px -50px;
			}
		}
	}
</style>
