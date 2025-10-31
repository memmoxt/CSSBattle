<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--green: #37a76f;
		--black: #000000;
        background-color:var(--black);
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
			height: 130px;
			width: 180px;
			translate: -110px -85px;
			background-color: var(--green);
			box-shadow:
				220px 0 var(--green),
				0px 170px var(--green),
				220px 170px var(--green);
			&:before {
				content: '';
				height: 60px;
				position: absolute;
				translate: 110px 60px;
				border-radius: 50%;
				aspect-ratio: 1;
				background-color: var(--green);
                box-shadow: 0 0 0 40px var(--black), 120px 120px var(--green), 120px 120px 0 40px var(--black);
			}
		}
	}
</style>
