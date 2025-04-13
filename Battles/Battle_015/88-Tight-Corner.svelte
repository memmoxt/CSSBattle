<div class="main">
	<div></div>
	<div></div>
</div>

<style>
* {
    margin: 0;
    padding: 0;
    box-sizing: content-box;
    --white: #f7f3da;
    --red: #d25b70;
}

.main {
    height: 300px;
    width: 400px;
    display: flex;
    justify-content: center;
    align-items: center;
    position: absolute;
    overflow: hidden;
    background-color: var(--white);

    &>div:nth-child(1),
    &>div:nth-child(2) {
        position: absolute;
        height: 20px;
        width: 20px;
        background-color: var(--red);
        transform: translate(10px, -10px);

        &:before {
            content: '';
            position: absolute;
            background-color: var(--red);
            height: 40px;
            width: 200px;
            transform: translate(0px, 20px);
            border-bottom-left-radius: 10px;
        }

        &:after {
            content: '';
            position: absolute;
            height: 150px;
            width: 200px;
            border-bottom-left-radius: 20px;
            left: 0px;
            bottom: 0px;
            background-color: var(--white);
            transform: translate(0px, 0px);
        }
    }

    &>div:nth-child(2) {
        transform: scale(-1) translate(10px, -10px);
    }

}
</style>
