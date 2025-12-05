
<div class="main">
	<div><div></div></div>

</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--green: #32955e;
		--white: #ffffff;
		--black: #000000;
        background-color: var(--green);
        
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		overflow: hidden;
		position: absolute;
		& > div {
			height: 140px;
			width: 200px;
			translate: 0 80px;
			background-color: var(--white);
			border-top-right-radius: 140px;
			border-top-left-radius: 70px;
            overflow:hidden;
            &>div{
                height: 40px;
                width: 80px;
                background-color:var(--green);
                translate: 150px 90px;
                border-radius: 50px/50px;
                &:before{
                    content:'';
                    position:absolute;
                    height: 20px;
                    border-radius:50%;
                    aspect-ratio:1;
                    background-color: var(--black);
                    translate: -20px -30px;

                }

            }
		}
	}
</style>
