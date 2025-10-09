<div class="main">
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--yellow: #f0cd48;
		--blue: #243d83;
		--teal: #5aa4b7;
        background-color: var(--yellow);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		overflow: hidden;
		position: absolute;
		& > div:nth-child(1) {
			position: absolute;
			height: 60px;
			width: 120px;
			background-color: var(--yellow);
			box-shadow: 0 0 0 60px var(--blue);
			z-index: 1;
		}
		& > div:nth-child(2) {
			position: absolute;
			height: 80px;
			background-color: var(--yellow);
			aspect-ratio: 1;
			translate: 80px -50px;
			z-index: 2;
            &:before{
                content:'';
                position:absolute;
                border-top: 30px solid transparent;
                border-right: 20px solid transparent;
                border-bottom: 30px solid transparent;
                border-left: 60px solid var(--teal);
            }
		}
	}
</style>
