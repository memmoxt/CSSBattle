<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--green: #7c9a81;
		--yellow: #fff9c6;
		--orange: #efcb5c;
        background-color:var(--green);
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
			height: 90px;
			width: 270px;
			border-radius: 50px/50px;
			background-color: var(--yellow);
            &:before{
                position:absolute;
                content:'';
                height:70px;
                aspect-ratio:1;
                background-color:var(--orange);
                border-radius:50%;
                top:115px;
                right:95px;
                box-shadow:0 0 0 30px var(--green);
            }
		}
	}
</style>
