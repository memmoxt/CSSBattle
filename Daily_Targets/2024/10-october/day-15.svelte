<div class="main">
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--green: #1a4341;
		--dark_green: #0b2429;
		--yellow: #998235;
		--gold: #f3ac3c;
        background-color:var(--dark_green);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		& > div {
			height: 180px;
			aspect-ratio: 1;
			background-color: var(--gold);
			opacity: 1;
			border-top-left-radius: 100px;
			border-bottom-right-radius: 100px;
			&:before {
				content: '';
				position: absolute;
				background-color: var(--yellow);
				height: 150px;
				aspect-ratio: 1;
				transform: translate(0px, 30px);
				border-top-left-radius: 100px;
				border-bottom-right-radius: 100px;
			}
			&:after {
				content: '';
				position: absolute;
				background-color: var(--green);
				height: 120px;
				aspect-ratio: 1;
				transform: translate(0px, 60px);
				border-top-left-radius: 100px;
				border-bottom-right-radius: 100px;
			}
		}
		& > div:nth-child(1) {
			transform: translate(-20px, 60px);
		}
        &>div:nth-child(2){
            transform:scale(-1) translate(-20px, 60px);
        }
	}
</style>

