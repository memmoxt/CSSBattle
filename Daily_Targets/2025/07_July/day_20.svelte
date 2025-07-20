<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--yellow: #fade8b;
		--green: #48bf7d;
		--white: #ffffff;
        background-color:var(--yellow);
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
			width: 140px;
			background-color: var(--green);
			border-radius: 50px/50px;
			translate: 0px 5px;
			box-shadow: 0px 40px var(--green);
			&:before {
				content: '';
				position: absolute;
				height: 100px;
				aspect-ratio: 1;
				border-radius: 50%;
				translate: 20px -50px;
				background-color: var(--green);
			}
			&:after {
				content: '';
				position: absolute;
				background-color: var(--white);
				height: 15px;
				border-radius: 50%;
				aspect-ratio: 1;
				translate: 43px -13px;
                box-shadow: 40px 0 var(--white);
			}
		}
	}
</style>
