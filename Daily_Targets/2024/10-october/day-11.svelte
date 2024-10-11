<div class="main">
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--blue: #6592cf;
		--darkblue: #243d83;
		--yellow: #eeb850;
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		& > div {
			height: 100%;
			width: 50%;
		}
		& > div:nth-child(1) {
			background-color: var(--yellow);
            &:before{
                height:100%;
                content:'';
                position:absolute;
                width:20%;
                background-color:var(--blue);
                transform:translateX(160px);
            }
		}
		& > div:nth-child(2) {
			background-color: var(--darkblue);
            &:before{
                height:50px;
                content:'';
                position:absolute;
                width:240px;
                background-color:var(--blue);
                transform:translateX(-50%);
                box-shadow: 0 250px 0 var(--blue);
            }
		}
	}
</style>

