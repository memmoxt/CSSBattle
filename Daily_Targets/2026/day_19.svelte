<div class="main">
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--orange: #de9473;
		--white: #f9eaf1;
		--black: #394257;
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		overflow: hidden;
		position: absolute;
        background-color: var(--orange);
		& > div {
			position: absolute;
			height: 140px;
			width: 140px;
			translate: -120px;
			background-color: var(--orange);
			border-top: 30px solid var(--white);
			border-right: 0px solid var(--white);
			border-bottom: 30px solid var(--white);
			border-left: 30px solid var(--white);
			&:before {
				content: '';
				position: absolute;
				height: 25px;
				width: 80px;
				background-color: var(--black);
				box-shadow: 0 55px var(--black);
			}
		}
        &>div:nth-child(2){
            transform:scale(-1);
            translate: 120px;
        }
	}
</style>
