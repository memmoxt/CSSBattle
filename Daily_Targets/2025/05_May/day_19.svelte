<div class="main">
	<div>
		<div></div>
		<div></div>
		<div></div>
	</div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--green: #bde4c1;
		--red: #d95f5b;
		--gray: #4c455b;
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		position: absolute;
		overflow: hidden;
        background-color:var(--green);
		& > div:nth-child(1) {
			justify-content: center;
			column-gap: 40px;
			height: 300px;
			width: 400px;
			display: grid;
			grid-template-columns: repeat(3, 80px);
			grid-template-rows: repeat(3, 1fr);
			& > div {
				position: relative;
				grid-column: 1/2;
				grid-row: 1/3;
				background-color: var(--gray);
				&:before {
					content: '';
					position: absolute;
					height: 80px;
					aspect-ratio: 1;
					border-radius: 50%;
					background-color: var(--red);
					transform: translateY(160px);
					clip-path: polygon(0px 40px, 0px 85px, 80px 85px, 80px 40px);
				}
			}
            &>div:nth-child(2){
                grid-column: -1/-2;
            }
            &>div:nth-child(3){
                grid-column:2/3;
                grid-row:-1/-3;
                transform:rotate(180deg);
                background-color:var(--red);
                &:before{
                    background-color:var(--gray);
                }
            }
		}
	}
</style>
