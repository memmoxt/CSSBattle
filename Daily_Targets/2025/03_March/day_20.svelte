<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--yellow: #d4ed33;
		--green: #1a353c;
        background-color:var(--yellow);
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
			height: 100%;
			transform: translate(-100px);
			width: 30px;
			background-color: var(--green);
			box-shadow:
				65px 0 0 var(--green),
				135px 0 0 var(--green),
				200px 0 0 var(--green);
            &:before{
                content:'';
                position:absolute;
                height:30px;
                width:50px;
                left:90px;
                top:135px;
                background-color:var(--green);
            }
		}
	}
</style>

