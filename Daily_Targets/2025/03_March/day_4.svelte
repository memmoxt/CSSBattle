<div class="main">
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--green: #4a9a86;
		--white: #ebf6f0;
        background-color:var(--white);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		flex-wrap: wrap;
		position: absolute;
		/* overflow: hidden; */
		& > div:nth-child(1) {
			position: absolute;
			height: 168px;
			border-radius: 50%;
			aspect-ratio: 1;
			background-color: var(--green);
			/* opacity: 0.5; */
			&:before {
				content: '';
				position: absolute;
				border-top: 150px solid transparent;
				border-right: 0px solid transparent;
				border-bottom: 150px solid transparent;
				border-left: 116px solid var(--green);
				top: -65px;
				left: -116px;
			}
			&:after {
				content: '';
				position: absolute;
				border-top: 150px solid transparent;
				border-right: 103px solid transparent;
				border-bottom: 150px solid transparent;
				border-left: 116px solid var(--green);
				top: -65px;
				left: -114px;
				transform: translate(180px) scale(-1);
			}
		}
        &>div:nth-child(2){
            position:absolute;
            height:100px;
            width:300px;
            background-color:var(--green);
        }
	}
</style>

