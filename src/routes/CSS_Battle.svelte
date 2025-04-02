<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--green: #5a9f48;
		--black: #394257;
        background-color: var(--green);
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
            transform:translate(0 ,-40px);
            height:80px;
            width:200px;
            background-color: var(--black);
            &:before{
                content:'';
                position: absolute;
                transform: translate(55px ,110px);
                height:120px;
                width:30px;
                background-color: var(--black);
                box-shadow: 60px 0 var(--black);
            }
            &:after{
                position: absolute;
                content: '';
                height:100px;
                aspect-ratio: 1;
                border-radius:50%;
                transform:translate(50px,30px);
                box-shadow:0 0 0 30px var(--black);
                background-color: var(--green);
            }
		}

	}
</style>
