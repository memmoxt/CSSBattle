<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--orange: #e8ad6d;
		--red: #de6b67;
        background-color:var(--orange);
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
		& > div {
			position: absolute;
			height: 300px;
			width: 40px;
			transform: translate(-96px);
			background-color: var(--red);
			box-shadow:
				60px 0 var(--red),
				100px 0 var(--red),
				130px 0 var(--red),
				191px 0 var(--red);
			/* opacity: 0.5; */
            &:before,&:after{
                content:'';
                position:absolute;
                background-color:var(--orange);
                width:42px;
                height:30px;
                transform:translate(94px, 79px);
                clip-path: polygon(50% 0px, 100% 50%, 50% 100%, 0 50%);
            }
            &:after{

                transform:translate(94px, 190px);
            }
		}
	}
</style>

