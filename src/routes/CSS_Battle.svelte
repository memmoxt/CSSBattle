<div class="main">
	<div>
		<div></div>
		<div></div>
		<div></div>
		<div></div>
		<div></div>
		<div></div>
		<div></div>
		<div></div>
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
		box-sizing: border-box;
        --red:#DE6B67; 
        --white:#FCEBEB;
        background-color:var(--white);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		overflow: hidden;
		position: absolute;
		& > div:nth-child(1) {
			height: 260px;
			width: 300px;
			display: grid;
			grid-template-columns: repeat(5, 1fr);
			grid-template-rows: repeat(13, 1fr);
            &>div{
				background-color: var(--red);
            }
			& > div:nth-child(odd) {
				grid-column: 3/4;
			}
			& > div:nth-child(even) {
			}
			& > div:nth-child(1) {
				grid-row: -1/-2;
			}
			& > div:nth-child(3) {
				grid-row: -3/-4;
			}
			& > div:nth-child(5) {
				grid-row: -5/-6;
			}
			& > div:nth-child(7) {
				grid-row: 5/6;
			}
			& > div:nth-child(9) {
				grid-row: 3/4;
			}
			& > div:nth-child(11) {
				grid-row: 1/2;
			}
			& > div:nth-child(2) {
				grid-area: 7/1/8/2;
			}
			& > div:nth-child(4) {
				grid-area: 6/2/7/3;
			}
			& > div:nth-child(6) {
				grid-area: 8/2/9/3;
			}
			& > div:nth-child(8) {
				grid-area: 8/4/9/5;
			}
			& > div:nth-child(10) {
				grid-area: 6/4/6/5;
			}
			& > div:nth-child(12) {
				grid-area: 7/5/8/6;
			}
		}
	}
</style>
