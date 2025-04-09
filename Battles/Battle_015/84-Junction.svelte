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
        box-sizing: content-box;
        --black: #191919;
        --dark: #a64942;
        --light: #fe5f55;
    }

    .main {
        height: 300px;
        width: 400px;
        display: flex;
        justify-content: center;
        align-items: center;
        position: absolute;
        overflow: hidden;
        background-color:var(--black);

        &>div {
            position:absolute;
            height: 130px;
            width: 40px;
            background-color: var(--light);
            transform:translateY(-85px);
            border-bottom-left-radius:20px;
            border-bottom-right-radius:20px;
            /* opacity: 0.5; */
        }
        &>div:nth-child(2){
            transform:rotate(180deg)translateY(-85px)
        }
        &>div:nth-child(3){
            height:180px;
            transform: translate(110px) rotate(90deg);
            background-color: var(--dark);
        }
        &>div:nth-child(4){
            height:180px;
            transform: translate(-110px) rotate(-90deg);
            background-color: var(--dark);
        }
    
    }
</style>
