<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--blue: #4f77ff;
		--white: #ffffff;
        background-color:var(--blue);
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
			height: 120px;
			aspect-ratio: 1;
            transform:translate(0px , 30px);
            background-color:var(--white);
            border-radius:50%;
            &:before{
                content:'';
                position:absolute;
                height:60px;
                width:20px;
                transform:translate(50px,-10px);
                background-color:var(--white);
                box-shadow:0 0 0 10px var(--blue);
            }
            &:after{
                content:'';
                position:absolute;
                height:20px;
                width:140px;
                transform:translate(-10px,-60px);
                background-color:var(--white);
                box-shadow:0 30px 0 var(--white);
            }
		}
	}
</style>

