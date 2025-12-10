<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--blue: #202f8e;
		--purple: #7982bb;
		--white: #ffffff;
        background-color:var(--blue);
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
			height: 50px;
			width: 100px;
			background-color: var(--purple);
            box-shadow: 130px 0 var(--purple), -130px 0 var(--white);
            border-radius:50px / 50px;
            &:before{
                content:'';
                position:absolute;
                height: 20px;
                width: 100px;
                background-color: var(--white);
                translate: -130px 60px;
            }
		}
	}
</style>
