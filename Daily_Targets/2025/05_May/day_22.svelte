<div class="main">
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--blue: #243d83;
		--white: #e3dcd1;
        background-color:var(--white);
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
            position:absolute;
			height: 600px;
			width: 60px;
			background-color: var(--blue);
			box-shadow:
				-135px 0 var(--blue),
				135px 0 var(--blue), 270px 0 var(--blue), -270px 0 var(--blue);
		}
        &>div:nth-child(1){
            
            transform:rotate(-45deg);
        }
	}
</style>
