<div class="main">
	<div></div>
</div>

<style>
    * {
        margin: 0;
        padding: 0;
        box-sizing: content-box;
        --orange: #f58220;
        --white: #ffffff;
    }

    .main {
        height: 300px;
        width: 400px;
        display: flex;
        justify-content: center;
        align-items: center;
        position: absolute;
        overflow: hidden;
        background-color:var(--orange);

        &>div {
            height: 100px;
            width: 260px;
            background-color: var(--orange);
            box-shadow:0 0 0 20px var(--white);
            /* opacity: 0.5; */
            &:before{
                content:'';
                position:absolute;
                height:180px;
                aspect-ratio:1;
                background-color:var(--orange);
                border-radius:50%;
                transform:translate(40px,-40px);
            }
            &:after{
                content:'';
                position:absolute;
                height:20px;
                width:300px;
                background-color:var(--white);
                transform:translate(-20px,40px);
            }
        }
    }
</style>

