<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--marine: #2b2a4a;
		--white: #ece3df;
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
			position: absolute;
			height: 150px;
			width: 260px;
			background-color: var(--marine);
			translate: 0px -100px;
            box-shadow: 0px 200px var(--marine);
			&:before {
				content: '';
				position: absolute;
				height: 25px;
				width: 80px;
				background-color: var(--marine);
                translate: 260px 125px;
                box-shadow: -340px 75px var(--marine);
			}
		}
	}
</style>
