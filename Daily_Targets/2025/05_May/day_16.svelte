<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--green: #5a9f48;
		--black: #000000;
        background-color:var(--green);
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
			height: 80px;
			transform: translate(0px, -55px);
			aspect-ratio: 1;
			border-radius: 50%;
			background-color: var(--green);
			box-shadow:
				0 0 0 30px var(--black),
                0px 110px var(--green),
                0 110px 0 30px var(--black),
                -30px 55px var(--green),
				30px 55px var(--green),
                -30px 55px 0 30px var(--black),
                30px 55px 0 30px var(--black);
                &:before{
                content:'';
                position:absolute;
                height:50px;
                aspect-ratio:1;
                background-color:var(--green);
                transform:translate(15px ,70px);
            }
		}
	}
</style>
