<div class="main">
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--green: #66dbb8;
		--darkgreen: #1a353c;
        background-color:var(--green);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		flex-wrap: wrap;
		position: absolute;
        overflow: hidden;
        
		& > div {
			top: 0px;
			position: absolute;
			height: 135px;
			width: 170px;
			background-color: var(--green);
			/* opacity: 0.5; */
			box-shadow:
				0 0 0 30px var(--darkgreen),
				0 165px 0 var(--green),
				0 165px 0 30px var(--darkgreen);
			&:before {
				content: '';
				position: absolute;
				height: 120px;
				aspect-ratio: 1;
				background-color: var(--darkgreen);
				border-radius: 50%;
				transform: translate(-75px, 90px);
				box-shadow: 200px 0 0 var(--darkgreen);
			}
            &:after{
                content:'';
                position:absolute;
				height: 60px;
				aspect-ratio: 1;
				background-color: var(--green);
				border-radius: 50%;
				transform: translate(-45px, 120px);
				box-shadow: 200px 0 0 var(--green);
            }
		}
	}
</style>

