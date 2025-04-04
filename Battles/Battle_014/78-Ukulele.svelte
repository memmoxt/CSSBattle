<div class="main">
	<div class="base"></div>
	<div class="body"></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--yellow: #f3ac3c;
		--darkyellow: #998235;
		--green: #1a4341;
	}

	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		position: absolute;
		overflow: hidden;
        background-color:var(--yellow);
		& > div {
			position: absolute;
		}
		& > .base {
			height: 20px;
			width: 150px;
			background-color: var(--green);
			/* opacity: 0.5; */
			transform: translate(50px);
			&:before {
				content: '';
				position: absolute;
				height: 30px;
				width: 40px;
				background-color: var(--darkyellow);
				transform: translate(140px, -5px);
				border-radius: 10px/10px;
			}
			&:after {
				content: '';
				position: absolute;
				height: 4px;
				width: 20px;
				transform: translate(150px, 3px);
				background-color: var(--green);
				box-shadow: 0 10px var(--green);
				border-radius: 2px;
			}
		}
		& > .body {
			height: 40px;
			border-radius: 50%;
			transform: translate(-35px);
			aspect-ratio: 1;
			background-color: var(--green);
			box-shadow:
				0 0 0 5px var(--yellow),
				0 0 0 30px var(--darkyellow),
                -60px 0 0 40px var(--darkyellow);
			/* opacity: 0.5; */
            &:before{
                content:'';
                position:absolute;
                background-color:var(--green);
                height:40px;
                width:10px;
                border-radius:5px;
                transform:translate(-60px);
                
            }
		}
	}
</style>

