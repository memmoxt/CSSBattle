<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--yellow: #eddf5a;
		--purple: #3e4071;
        background-color:var(--yellow);
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
			height: 170px;
			width: 40px;
			translate: 0 -35px;
			background-color: var(--purple);
			&:before {
				content: '';
				position: absolute;
				height: 40px;
				width: 280px;
				background-color: var(--purple);
				translate: -120px 200px;
			}
			&:after {
				content: '';
				position: absolute;
				height: 200px;
				width: 200px;
				background-color: var(--purple);
                translate:-80px;
                clip-path:polygon(1px 92px, 100px 190px, 200px 92px, 172px 63px, 120px 115px, 80px 115px, 30px 64px);
			}
		}
	}
</style>
