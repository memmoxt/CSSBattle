<div class="main">
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--red: #ac5353;
		--black: #222222;
        background-color: var(--red);
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
			position: absolute;
			height: 180px;
			aspect-ratio: 1;
			background-color: var(--black);
			translate: 0 40px;
			border-radius: 50%;
			&:before {
				content: '';
				position: absolute;
				height: 20px;
				aspect-ratio: 1;
				background-color: var(--black);
				border-radius: 50%;
				translate: 80px -80px;
			}
			&:after {
				content: '';
				position: absolute;
				height: 80px;
				width: 10px;
				background-color: var(--black);
				translate: 85px -70px;
			}
		}
        &>div:nth-child(2){
            position:absolute;
            height: 60px;
            aspect-ratio:1;
            background-color: var(--black);
            translate: -60px -80px;
            border-radius: 50%;
            box-shadow: 120px 0px var(--black);
            &:before{
                content:'';
                position:absolute;
                height: 10px;
                width: 100px;
                background-color: var(--black);
                translate: 40px 25px;
            }
        }
	}
</style>
