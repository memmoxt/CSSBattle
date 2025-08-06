<div class="main">
	<div>
		<div></div>
		<div></div>
		<div></div>
		<div></div>
	</div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		/* box-sizing: content-box; */
		box-sizing: border-box;
		--blue: #88ebf8;
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
		& > div {
			height: 300px;
			width: 400px;
			display: grid;
			grid-template-columns: repeat(2, 1fr);
			grid-template-rows: repeat(2, 1fr);
			justify-content: center;
			align-items: center;
			gap: 20px;
			& > div {
				background-color: var(--blue);
				height: 140px;
				width: 200px;
				z-index: 2;
			}
			& > div:nth-child(2),
			& > div:nth-child(3) {
				&:before {
					content: '';
					position: absolute;
					height: 30px;
					aspect-ratio: 1;
					border-radius: 50%;
					translate: -5px 55px;
					background-color: var(--blue);
					box-shadow: 0 0 0 20px var(--dark);
				}
                &:after{
                    content:'';
                    position:absolute;
                    height:150px;
                    width:20px;
                    background-color:var(--dark);
                    translate:-20px;
                }
				z-index: 1;
			}
            &>div:nth-child(3){
                transform:rotate(180deg);
            }
		}
	}
</style>
