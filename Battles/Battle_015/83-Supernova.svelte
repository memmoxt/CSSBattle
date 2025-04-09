<div class="main">
	<div></div>
</div>

<style>
    * {
        margin: 0;
        padding: 0;
        box-sizing: content-box;
        --darkblue: #243d83;
        --lightblue: #6592cf;
        --yellow: #eeb850;
    }

    .main {
        height: 300px;
        width: 400px;
        display: flex;
        justify-content: center;
        align-items: center;
        position: absolute;
        overflow: hidden;
        background-color:var(--darkblue);

        &>div {
            height: 100px;
            aspect-ratio: 1;
            position: absolute;
            border-radius: 50%;
            /* opacity: 0.5; */
            background-color: red;
            box-shadow: 60px 0 var(--lightblue), -60px 0 var(--lightblue), 0 60px var(--lightblue), 0 -60px var(--lightblue);
            transform: rotate(45deg);

            &:before {
                content: '';
                position: absolute;
                transform: translate(-10px, -10px);
                height: 120px;
                aspect-ratio: 1;
                background-color: var(--darkblue);
            }
            &:after{
                content: '';
                position: absolute;
                transform: translate(20px, 20px);
                border-radius:50%;
                height: 60px;
                aspect-ratio: 1;
                background-color: var(--yellow);

            }

        }
    }
</style>
