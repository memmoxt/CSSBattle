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
	</div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
        --yellow:#eeb850;
        --lightblue:#6592cf;
        --blue:#243d83;
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
        background-color:var(--lightblue);
		& > div {
			height: 180px;
			width: 280px;
			display: grid;
			justify-items: center;
			align-content: center;
            row-gap: 45px;
            column-gap:35px;
			grid-template-rows: repeat(3, 1fr);
			grid-template-columns: repeat(3, 1fr);
			& > div{
				height: 30px;
				width: 70px;
			}
            &>div:nth-child(odd){
                background-color:var(--yellow);
            }
            &>div:nth-child(even){
                background-color:var(--blue);
            }
		}
	}
</style>

