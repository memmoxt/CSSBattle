<div class="main">
	<div></div>
	<div></div>
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--gray: #3f4869;
		--black: #242a42;
		--green: #61a74e;
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		flex-wrap: wrap-reverse;
		flex-direction: column;
        background-color:var(--gray);
		& > div:nth-child(1) {
			position: absolute;
			height: 217px;
			width: 182px;
			background-color: var(--green);
			border-radius: 50%;
		}
		& > div:nth-child(2) {
			position: absolute;
			height: 120px;
			transform: translateY(58px) rotate(45deg);
			aspect-ratio: 1;
			background-color: var(--green);
			border-radius: 45px;
		}
        &>div:nth-child(3),&>div:nth-child(4){
            position:absolute;
            height:60px;
            width:40px;
            border-radius:50%;
            transform:translateX(-50px) translateY(29px) rotate(-50deg);
            background-color:var(--black);
        }
        &>div:nth-child(4){
            transform:translateX(50px) translateY(29px) rotate(50deg);
        }
	}
</style>

