<div class="main">
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--dark: #186d37;
		--light: #48bf7d;
        background-color:var(--dark);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		position: absolute;
		overflow: hidden;
		& > div:nth-child(1),
		div:nth-child(2) {
			position: absolute;
			height: 50px;
			width: 140px;
			background-color: var(--light);
			&:before {
				content: '';
				position: absolute;
				width: 50px;
				height: 140px;
				background-color: var(--light);
				transform: translate(45px, -45px);
			}
			&:after {
				content: '';
				position: absolute;
				width: 100px;
				aspect-ratio: 1;
				background-color: var(--dark);
				transform: translate(20px, -25px);
			}
		}
        &>div:nth-child(1){
            z-index:2;
        }
        &> div:nth-child(2){
            transform:scale(2) rotate(-45deg);
            z-index:1;
        }
	}
</style>
