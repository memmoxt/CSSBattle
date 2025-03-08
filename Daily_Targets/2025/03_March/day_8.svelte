<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--green: #498488;
		--red: #d99795;
		--white: #d9d9d9;
        background-color:var(--green);
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
			height: 140px;
			width: 240px;
			background-color: var(--red);
			/* opacity: 0.5; */
            &:before{
                position:absolute;
                content:'';
                height:110px;
                aspect-ratio:1;
                background-color:var(--green);
                border-radius:50%;
                top:160px;
                left:30px;
                box-shadow:230px 0 var(--green);
            }
            &:after{
                position:absolute;
                content:'';
                height:20px;
                width:240px;
                background-color:var(--white);
            }
		}
	}
</style>

