<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
        --blue:#434b92;
        --yellow:#eac049;
        background-color:var(--blue);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		flex-wrap: wrap-reverse;
		flex-direction: column;
    
        &>div{
            height:30px;
            width:200px;
            transform:translate(80px,-105px);
            box-shadow: -140px 30px 0 0 var(--yellow),
                -20px 60px 0 0 var(--yellow),
                -120px 90px 0 0 var(--yellow),
                -40px 120px 0 0 var(--yellow),
                -100px 150px 0 0 var(--yellow),
                -60px 180px 0 0 var(--yellow),
                -80px 210px 0 0 var(--yellow);
            background-color:var(--yellow);
        }
	}
</style>

