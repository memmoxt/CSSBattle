<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--blue: #558c90;
		--green: #325853;
        background-color:var(--blue);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		& > div {
			height: 100px;
			aspect-ratio: 1;
			background-color: var(--green);
            &:before{
                content:'';
                position:absolute;
                height:30px;
                width:200px;
                background-color:var(--green);
                transform:translate(-50px,-50px);
                box-shadow:0px 170px 0 0 var(--green);
            }
		}
	}
</style>

