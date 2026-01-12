<div class="main">
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--yellow: #fade8b;
		--black: #222222;
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
			height: 180px;
			width: 160px;
			background-color: var(--black);
			&:before,
			&:after {
				--quarter-value: 60px;
				position: absolute;
				content: '';
				border-top: var(--quarter-value) solid transparent;
				border-right: var(--quarter-value) solid transparent;
				border-bottom: var(--quarter-value) solid transparent;
				border-left: var(--quarter-value) solid transparent;
				border-radius: 50%;
				box-shadow: 0 0 0 var(--quarter-value) var(--black);
				clip-path: polygon(-120px 0px, 60px -120px, 60px 60px, -120px 60px);
				translate: -60px 60px;
			}
			&:after {
				translate: 100px 60px;
				transform: scaleX(-1);
			}
		}
        &> div:nth-child(2){
            position:absolute;
            height: 120px;
            width:40px;
            background-color: var(--yellow);
            translate:0 -30px;
        }
	}
</style>
