<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--green: #5a9f48;
		--white: #ffffff;
        background-color:var(--white);
	}

	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		position: absolute;
		overflow: hidden;
		& > div {
			position: absolute;
			height: 240px;
			border-radius: 50%;
			aspect-ratio: 1;
			background-color: var(--green);
			&:before {
				position: absolute;
				content: '';
				height: 40px;
				aspect-ratio: 1;
				background-color: var(--white);
				transform: translate(79px, 149px) rotate(45deg);
			}
            &:after{
                position:absolute;
                content:'';
                height:140px;
                width:40px;
				background-color: var(--white);
				transform: translate(135px, 85px) rotate(45deg);
            }
		}
	}
</style>
