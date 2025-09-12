<div class="main">
	<div></div>
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--yellow: #f0cd48;
		--dark: #23384b;
        background-color:var(--dark);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		overflow: hidden;
		position: absolute;
		& > div:nth-child(1) ,&>div:nth-child(2){
            position: absolute;
			height: 105px;
			width: 40px;
			translate: -70px 17px;

			&:before {
				content: '';
				position: absolute;
				width: 40px;
				aspect-ratio: 1;
				border-radius: 50%;
				translate: -0px -15px;
				box-shadow: 0 0 0 20px var(--yellow);
				clip-path: polygon(-50px -30px, 70px -30px, 70px 20px, -50px 20px);
			}
			&:after {
				content: '';
				position: absolute;
				height: 105px;
				width: 80px;
				translate: -20px 0px;
				background-color: var(--yellow);
				clip-path: polygon(
					-20px 5px,
					80px 5px,
					80px 25px,
					60px 25px,
					60px 5px,
					20px 5px,
					20px 105px,
					-20px 105px
				);
			}
		}
        &>div:nth-child(2){
            transform:scaleX(-1);
            translate: 70px 17px;
        }
        &>div:nth-child(3){
            position:absolute;
            height:100px;
            border-radius:50%;
            translate:0px -10px;
            aspect-ratio:1;
            background-color:var(--yellow);
            clip-path:polygon(0 50px, 100% 50px, 100% 100%, 0 100%);
        }
	}
</style>
