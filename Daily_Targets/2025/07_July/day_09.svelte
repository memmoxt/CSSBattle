<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--black: #2e312b;
		--white: #d9d9d9;
		--green: #7aa70a;
		background-color: var(--white);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		overflow: hidden;
		& > div {
			height: 40px;
			aspect-ratio: 1;
			background-color: var(--black);
			box-shadow: 0px 0 0 20px var(--green);
			&:before {
				content: '';
				position: absolute;
				height: 110px;
				width: 160px;
				translate: 60px 60px;
				box-shadow:
					-240px 0 var(--black),
					-240px -190px var(--black),
					0px -190px var(--black);
				background-color: var(--black);
			}
		}
	}
</style>
