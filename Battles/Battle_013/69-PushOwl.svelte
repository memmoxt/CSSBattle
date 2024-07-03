<div class="main">
	<div class="eye-left">
		<div class="pupil"></div>
	</div>
	<div class="eye-right">
		<div class="pupil"></div>
	</div>
    <div class="beak"></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--orange: #e08027;
		--yellow: #f2ad43;
		--brown: #824b20;
		--black: #191919;
	}

	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
        background:var(--black);
		& > .eye-left , &> .eye-right{
            position:absolute;
			height: 114px;
			aspect-ratio: 1;
			border-radius: 0 50% 50% 50%;
			background: var(--orange);
			transform: translate(-54px, -16px);
			display: flex;
			justify-content: center;
			align-items: center;
            z-index:1;
			&:before {
				content: '';
				position: absolute;
				height: 90px;
				border-radius: 50%;
				aspect-ratio: 1;
				top: 12px;
				left: 12px;
				background-color: var(--black);
			}
			& > .pupil {
                position:absolute;
                transform:translateY(6px);
				height: 12px;
				aspect-ratio: 1;
				border-radius: 50%;
                border:9px solid var(--orange);
				background-color: var(--black);
                &:before{
                    content:"";
                    position:absolute;
                    height:15px;
                    width:30px;
                    background-color:var(--black);
                    transform:translate(-9px, 6px);
                }
			}
		}
        &>.eye-right{
            transform:scaleX(-1) translate(-54px , -16px);
            box-shadow: 0 0 0 10px var(--black);
        }
        &>.beak{
            height:50px;
            position:absolute;
            aspect-ratio:1;
            background-color:var(--orange);
            transform:rotate(45deg);
            top:162px;
            z-index: 0;
        }
	}
</style>

