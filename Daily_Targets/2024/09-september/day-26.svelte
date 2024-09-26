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
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		--purple: #434b92;
		--yellow: #f3ac3c;
		--black: #000000;
        background-color:var(--purple);
		& > div:nth-child(1), &>div:nth-child(2) {
            position:absolute;
			background-color: var(--yellow);
            height:175px;
            width:30px;
            left:125px;
            top:40px;
		}
        &>div:nth-child(2){
            left:245px;
        }
        &>div:nth-child(3){
            position:absolute;
            top:172px;
            height:300px;
            aspect-ratio:1;
            background-color:var(--yellow);
            border-radius:50%;
            clip-path: polygon( 0 0 , 300px 0px , 300px 45.5px, 0 45.5px);
            z-index: 1;
        }
        &>div:nth-child(4){
            height:40px;
            aspect-ratio:1;
            background-color:var(--black);
            border-radius:50%;
            transform:translate(-40px,65px);
            box-shadow: 80px 0 0 var(--black);
            z-index: 0;
        }
	}
</style>

