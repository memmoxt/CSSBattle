<div class="main">
	<div><div></div></div>
	<div><div></div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--yellow: #fade8b;
		--green: #61a74e;
		--blue: #243d83;
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
        background-color:var(--yellow);
		& > div {
			position: absolute;
			left: 90px;
			height: 120px;
			width: 180px;
            display:flex;
            justify-content: center;
            align-items:center;
            overflow: hidden;
            z-index:1;
			& > div {
				height: 180px;
                border-radius:50%;
				aspect-ratio: 1;
                background-color:var(--blue);
			}
		}
        &>div:nth-child(2){
            z-index:0;
            transform:translateX(40px);
            &>div{
                background-color:var(--green);
            }
        }
	}
</style>

