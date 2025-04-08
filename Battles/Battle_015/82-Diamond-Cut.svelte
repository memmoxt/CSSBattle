<div class="main">
	<div></div>
</div>

<style>
    * {
    margin: 0;
    padding: 0;
    box-sizing: content-box;
    --yellow: #f3ac3c;
    --amber: #998235;
    --green: #1a4341;
}

.main {
    height: 300px;
    width: 400px;
    display: flex;
    justify-content: center;
    align-items: center;
    position: absolute;
    overflow: hidden;
    background-color:var(--yellow);

    &>div {
        position: absolute;
        height: 100px;
        aspect-ratio: 1;
        background-color: var(--yellow);
        transform: translate(-2px, 0px) rotate(-45deg);
        box-shadow:0 0 0 30px var(--amber);
        /* opacity: 0.5; */

        &:before {
            content: '';
            position: absolute;
            transform:translate(50px);
        }

        &:after {
            content: '';
            position: absolute;
            height: 30px;
            aspect-ratio: 1;
            transform: translate(35px, 35px);
            background-color: var(--green);
            box-shadow: 0px -65px var(--yellow), 65px 0px var(--yellow);

        }
    }
}

</style>
