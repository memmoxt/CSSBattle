
<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--yellow: #fbfdb7;
		--green: #46ba67;
		--red: #d95362;
		background-color: var(--yellow);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		position: absolute;
		overflow: hidden;

		& > div {
			position: absolute;
			height: 180px;
			width: 60px;
			left: 60px;
			top: 0px;
			background-color: var(--green);
			box-shadow: 0 150px 0 0 var(--red);
			&:before {
				content: '';
				position: absolute;
				height: 185px;
				width: 60px;
				background-color: var(--green);
				bottom: -125px;
				right: -220px;
				box-shadow: 0 -150px var(--red);
			}
			&:after {
				content: '';
				position: absolute;
				height: 60px;
				width: 200px;
				top: 120px;
				left: 50px;
				background-color: var(--green);
			}
		}
	}
</style>
