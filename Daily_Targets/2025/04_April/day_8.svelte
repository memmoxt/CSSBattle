<div class="main">
	<div></div>
	<div></div>
</div>

<style>
* {
    margin: 0;
    padding: 0;
    box-sizing: content-box;
    --green: #5a9f48;
    --dark: #14576b;
}

.main {
    height: 300px;
    width: 400px;
    display: flex;
    justify-content: center;
    align-items: center;
    position: absolute;
    overflow: hidden;
    background-color: var(--dark);


    &>div {
        position: absolute;
        height: 140px;
        width: 140px;
        background-color: var(--green);

        &:before {
            content: '';
            position: absolute;
            height: 100px;
            width: 20px;
            transform: translate(-34px, 20px);
            box-shadow:188px 0 var(--green);
            background-color: var(--green);
        }

        &:after {
            content: '';
            transform: translate(-68px, 40px);
            position: absolute;
            height: 60px;
            width: 20px;
            box-shadow: 256px 0 var(--green);
            background-color: var(--green);

        }
    }
    &>div:nth-child(2){
        transform:rotate(90deg);
    }
}
</style>
