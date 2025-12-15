<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--green: #0b2429;
		--orange: #ce6f4a;
        background-color: var(--green);
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
			height: 170px;
			width: 220px;
			background-color: var(--orange);
			translate: 0px 15px;
			border-radius: 20px;
			&:before {
				content: '';
				position: absolute;
				height: 200px;
				width: 140px;
				background-color: var(--orange);
				translate: 0 -30px;
				border-radius: 20px;
			}
			&:after {
				content: '';
				position: absolute;
				height: 20px;
                width: 220px;
                translate: 0px 30px;
                background-color: var(--green);
			}
		}
	}
</style>
