<div class="main">
	<div></div>
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--purple: #2b2a4a;
		--orange: #de9473;
	}

	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		position: absolute;
        background-color:var(--purple);
		& > div:nth-child(1),&>div:nth-child(2) {
			height: 40px;
			width: 162px;
			transform: translateY(20px);
			overflow: hidden;
			position: absolute;
			&:before {
				content: '';
				position: absolute;
				height: 162px;
				aspect-ratio: 1;
				background-color: var(--orange);
				border-radius: 50%;
				transform: translateY(-40px);
			}
		}
		& > div:nth-child(2) {
			transform: scale(-1) translateY(20px);
		}
        &>div:nth-child(3){
            height:40px;
            width:160px;
            background-color:var(--orange);
            transform:translateY(90px);
            box-shadow:0 -180px var(--orange);
        }
	}
</style>

