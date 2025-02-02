<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--white: #eed9d9;
		--blue: #469dba;
		--purple: #46487c;
		background-color: var(--white);
	}

	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		position: absolute;
		& > div {
			height: 60px;
			width: 280px;
			background-color: var(--blue);
			&:before {
				content: '';
				position: absolute;
				height: 60px;
				aspect-ratio: 1;
				background-color: var(--blue);
				top: 60px;
				box-shadow: 220px 120px var(--blue);
			}
			&:after {
				content: '';
				position: absolute;
				height: 120px;
				aspect-ratio: 1;
				background-color: var(--purple);
				border-radius: 50%;
				bottom: 0px;
				left: 140px;
			}
		}
	}
</style>
