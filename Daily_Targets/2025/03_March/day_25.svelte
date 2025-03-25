<div class="main">
	<div></div>
	<div class="number2"></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--red: #e35158;
		--white: #d9d9d9;
        background-color:var(--red);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		flex-wrap: wrap;
		position: absolute;
		overflow: hidden;
		& > div:nth-child(1) {
			height: 40px;
			aspect-ratio: 1;
			background-color: var(--red);
			border-radius: 50%;
			position: absolute;
			transform: translate(0px, -64px);
			box-shadow: 0 0 0 36px var(--white);
            z-index:3;
		}
		&>.number2 {
			position: absolute;
			background-color: var(--white);
            transform:translate(0, 8px);
			height: 210px;
			width: 40px;
            z-index:1;
            &:before{
                content:'';
                position:absolute;
                height:30px;
                aspect-ratio:1;
                background-color:var(--white);
                transform:translate(40px,163px);
            }
            &:after{
                content:'';
                position:absolute;
                height:14px;
                aspect-ratio:1;
                background-color:var(--white);
                transform:translate(40px,139px);
            }
		}
	}
</style>

