<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
        --white:#F9FAFD;
        --lightblue:#A7C2FA;
        --blue:#4F73D9;
        background-color:var(--white);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		overflow: hidden;
		position: absolute;
        &>div{
            position:absolute;
            height: 160px;
            aspect-ratio:1;
            background-color: var(--lightblue);
            border-radius:50%;
            overflow:hidden;
            &:before{
                content:'';
                position:absolute;
                height: 60px;
                aspect-ratio:1;
                background-color:var(--blue);
                border-radius:50%;
                translate: 50px 20px;
            }
            &:after{
                content:'';
                position:absolute;
                height: 100px;
                width:120px;
                background-color:var(--blue);
                translate: 20px 92px;
                border-radius: 80px/75px;
            }
        }
	}
</style>
