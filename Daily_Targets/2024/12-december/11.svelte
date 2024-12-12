<div class="main">
	<div></div>
	<div></div>
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--white: #fff6d2;
		--gray: #67645e;
		--orange: #e88933;
	}

	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		overflow: hidden;
		position: absolute;
        background-color:var(--white);
		& > div:nth-child(1) {
			position: absolute;
			background-color: var(--white);
			height: 152px;
			aspect-ratio: 1;
			border-radius: 5px/5px;
		}
		& > div:nth-child(2) {
			background-color: var(--gray);
			height: 180px;
			aspect-ratio: 1;
			border-radius: 20px/20px;
		}
		& > div:nth-child(3),
		& > div:nth-child(3):before,
		& > div:nth-child(4),
		& > div:nth-child(4):before {
			content: '';
			top: 40px;
			position: absolute;
			height: 20px;
			width: 14px;
			border-top-left-radius: 7px;
			border-top-right-radius: 7px;
			background-color: var(--orange);
			box-shadow:
				30px 0px var(--orange),
				60px 0 var(--orange),
				-30px 0 var(--orange),
				-60px 0 var(--orange);
		}
		& > div:nth-child(3):before {
			transform: rotate(90deg) translate(60px, -100px);
		}
		& > div:nth-child(4):before {
			transform: rotate(90deg) translate(60px, -100px);
		}
        &>div:nth-child(4){
            transform:scale(-1) translate(0px, -200px);
        }
	}
</style>

