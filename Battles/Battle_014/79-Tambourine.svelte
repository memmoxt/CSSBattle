<div class="main">
	<div class="center-piece"></div>
	<div class="pieces"></div>
	<div class="pieces"></div>
	<div class="pieces"></div>
	<div class="pieces"></div>
	<div class="pieces"></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--dark: #243d83;
		--light: #6592cf;
        background-color:var(--light);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		position: absolute;
		overflow: hidden;
		& > div.pieces{
			position: absolute;
			height: 10px;
            border-radius:50%;
			aspect-ratio: 1;
			background-color: var(--dark);
            /* opacity:0.5; */
            box-shadow:0 0 0 10px var(--light), 0 0 0 20px var(--dark);
		}
        & > div:nth-child(2).pieces{
            transform:translate(-70px,-30px);
        }
        & > div:nth-child(3).pieces{
            transform:translate(-0px,-70px);
        }

        & > div:nth-child(4).pieces{
            transform:translate(70px,-30px);
        }
        & > div:nth-child(5).pieces{
            transform:translate(70px,40px);
        }
        & > div:nth-child(6).pieces{
            transform:translate(-70px,40px);
        }
		& > div.center-piece {
			position: absolute;
			height: 170px;
			aspect-ratio: 1;
			background-color: var(--dark);
			border-radius: 50%;
			/* opacity: 0.5; */
			transform: translateY(10px);
			overflow: hidden;
			&:before {
				content: '';
				position: absolute;
				height: 150px;
				aspect-ratio: 1;
				background-color: var(--light);
				border-radius: 50%;
				transform: translate(10px, 10px);
			}
			&:after {
				content: '';
				position: absolute;
				height: 100px;
				aspect-ratio: 1;
				border-radius: 50%;
				background-color: var(--light);
				transform: translate(35px, 135px);
				box-shadow: 0 0 0 10px var(--dark);
			}
		}
	}
</style>

