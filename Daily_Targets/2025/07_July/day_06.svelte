<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--black: #556d7f;
		--yellow: #fade8b;
        background-color:var(--black);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		overflow: hidden;
        
		& > div {
			height: 140px;
			width: 150px;
			background-color: var(--yellow);
			&:before {
				content: '';
				position: absolute;
				height: 50px;
				width: 65px;
				background-color: var(--yellow);
				translate: -65px 45px;
				box-shadow:
					-85px 0 var(--yellow),
					215px 0 var(--yellow),
					300px 0 var(--yellow);
			}
		}
	}
</style>
