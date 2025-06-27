<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--black: #394257;
		--red: #d24444;
        background-color:var(--black);
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
			height: 120px;
			aspect-ratio: 1;
			translate: -60px -70px;
			background-color: var(--red);
			box-shadow:
				120px 80px var(--red),
				0px 160px var(--red);
			&::before {
				content: '';
				position: absolute;
				height: 80px;
				aspect-ratio: 1;
				translate: 40px 40px;
				box-shadow:
					80px 80px var(--black),
					0px 160px var(--black);
				background-color: var(--black);
			}
		}
	}
</style>
