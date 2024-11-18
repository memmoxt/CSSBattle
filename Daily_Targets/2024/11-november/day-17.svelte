<div class="main">
	<div></div>
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--white: #ffffff;
		--red: #d96c7b;
	}
	.main {
        background-color:var(--red);
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		& > div {
			position: absolute;
			height: 90px;
			aspect-ratio: 1;
			background-color: var(--white);
			&:before {
				position: absolute;
				content: '';
				height: 30px;
				aspect-ratio: 1;
				right: 30px;
				top: 30px;
				background-color: var(--red);
			}
		}
		& > div:nth-child(2) {
			top: 35px;
			left: 85px;
			height: 100px;
			border-radius: 50%;
			aspect-ratio: 1;
            border-bottom-right-radius:0;
			&:before {
				right: 30px;
				height: 40px;
				border-radius: 50%;
			}
		}
		& > div:nth-child(3) {
			bottom: 35px;
			right: 85px;
			height: 100px;
			border-radius: 50%;
			aspect-ratio: 1;
            border-bottom-right-radius:0;
            transform:scale(-1);
			&:before {
				right: 30px;
				height: 40px;
				border-radius: 50%;
			}
		}
	}
</style>

