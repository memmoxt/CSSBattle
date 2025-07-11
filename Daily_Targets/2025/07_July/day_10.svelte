<div class="main">
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--green: #7aa70a;
		--white: #ffffff;
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		overflow: hidden;
        background-color:var(--green);
		& > div:nth-child(1) {
			height: 40px;
			width: 170px;
			background-color: var(--white);
			translate: 0 -90px;
            border-top-right-radius:50px;
            border-top-left-radius:50px;
            &:before{
                content:'';
                position:absolute;
                height:40px;
                width: 40px;
                background-color:var(--white);
                translate:0px 40px;
            }
            &:after{
                content:'';
                position:absolute;
                height: 40px;
                width:130px;
                background-color: var(--white);
                translate:0px 80px;
                border-bottom-left-radius:35px;
                border-top-right-radius:50px;

            }
		}
        &>div:nth-child(2){
            height:60px;
            aspect-ratio:1;
            background-color:var(--green);
            position:absolute;
            translate:15px 40px;
            border-radius:50%;
            box-shadow: 0 0 0 40px var(--white);
            &:before{
                content:'';
                position:absolute;
                height:40px;
                width: 120px;
                background-color:var(--white);
                translate:-70px 60px;
                border-bottom-left-radius:50px;
                border-bottom-right-radius:20px;
            }
            &:after{
                content:'';
                position:absolute;
                background-color: var(--green);
                height:60px;
                width:150px;
                translate:-120px 0px;
            }
        }
	}
</style>
