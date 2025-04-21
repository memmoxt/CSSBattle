<div class="main">
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--dark: #4c455b;
		--red: #d96c7b;
		--green: #8ab8b6;
	}

	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		position: absolute;
		& > div {
			height: 150px;
			width: 400px;
            overflow: hidden;
			background-color:var(--dark);
            position:absolute;
			align-self: flex-start;
			&:before {
				content: '';
				position: absolute;
                height:160px;
                aspect-ratio:1;
                background-color:var(--red);
                /* opacity:0.5; */
                border-radius:50%;
                transform:translate(120px,70px);
			}
            &:after{
                content:'';
                position:absolute;
                height:60px;
                aspect-ratio:1;
                background-color:var(--red);
                transform:translate(60px,30px);
                box-shadow:-60px 0 var(--red),0 60px var(--red);
            }
		}
        &>div:nth-child(2){
			align-self: flex-end;
            transform:scale(-1) translate(0px,0px);
            &:before{
                background-color:var(--green);
            }
            &:after{
                background-color:var(--green);
                box-shadow:-60px 0 var(--green),0 60px var(--green);
            }
        }
	}
</style>

