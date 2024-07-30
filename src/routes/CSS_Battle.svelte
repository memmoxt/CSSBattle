<div class="main">
	<div></div>
    <div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
        --blue:#4f77ff;
        --white:#eff8fe;
        background-color:var(--blue);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
        &>div:nth-child(1){
            height:200px;
            width:200px;
            border-radius:50%;
            background-color:red;
            background-color:var(--white);
            clip-path: polygon(0 100px, 0px 200px , 200px 200px, 200px 100px);
            z-index:2;
        }
        &>div:nth-child(2){
            height:200px;
            width:40px;
            background-color:var(--white);
            position:absolute;
            z-index:1;
            clip-path: polygon(0 150px, 0px -200px , 200px -200px, 200px 100px);
            transform:rotate(45deg);
        }
	}
</style>
