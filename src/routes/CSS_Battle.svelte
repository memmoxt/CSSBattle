<div class="main">
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		/* box-sizing: content-box; */
		box-sizing: border-box;
		--black: #423f36;
		--yellow: #feff58;
		--red: #d94e4e;
		--blue: #3e5aa9;
        background-color:var(--black);
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
			height: 100px;
			width: 400px;
			background-color: var(--yellow);
			&:before,
			&:after {
				content: '';
				position: absolute;
				translate: -125px 20px;
				height: 60px;
				width: 250px;
				border-radius: 50%;
				background-color: var(--red);
			}
			&:after {
				translate: 275px 20px;
				background-color: var(--blue);
			}
		}
        &>div:nth-child(2){
            position:absolute;
            height:102px;
            aspect-ratio:1;
            background-color:var(--black);
            border-radius:20px;
            transform:translateY(72px) rotate(-45deg);
        }
	}
</style>
