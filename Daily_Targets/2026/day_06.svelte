<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--white: #f3ead2;
		--green: #38483c;
		--red: #c36768;
        background-color: var(--white);
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
			height: 40px;
			aspect-ratio: 1;
			background-color: var(--green);
			box-shadow:
				0 0 0 10px var(--green),
				-110px 0 var(--green),
				110px 0 var(--green),
				0 -110px var(--green),
				0 110px var(--green);
			&:before {
				content: '';
				position: absolute;
				height: 60px;
				width: 40px;
				background-color: var(--red);
				translate: 0 -70px;
				box-shadow: 0 120px var(--red);
			}
			&:after {
				content: '';
				position: absolute;
				height: 40px;
				width: 60px;
				background-color: var(--red);
				translate: 50px 0;
				box-shadow: -120px 0 var(--red);
			}
		}
	}
</style>
