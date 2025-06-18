<script>
    export let buttonType;
    
</script>
<button class = {buttonType.class}>{buttonType.title}</button>
<style>
    .LoginBtn{
        background-color: #F5F7FA;
        color: #4CAF4F;
        width: 77px;
        height: 40px;
        padding: 10px 20px;
        border: none;
        font-size: 16px;
        line-height: 20px;
        letter-spacing: 0.1%;
        margin-left: 8.68%;
        transition: background-color 0.4s ease;
        font-weight: 500;
    }
    .LoginBtn:hover{
        background-color: #4CAF4F;
        color: #F5F7FA;
    }
    .LoginBtn:active{
        background-color: #ebecee;
        color: #4CAF4F;
    }
    .SignBtn{
        width: 91px;
        height: 40px;
        margin-left: 14px;
        border-radius: 6px;
        border: none;
        background-color: #4CAF4F;
        color: #F5F7FA;
        font-size: 16px;
        line-height: 20px;
        letter-spacing: 0.1%;
        transition: background-color 0.4s ease;
        font-weight: 500;
    }
    .SignBtn:hover{
        background-color: #F5F7FA;
        color: #4CAF4F;
    }
    .SignBtn:active{
        background-color: #4CAF4F;
        color: #F5F7FA;
    }
    .RegisterBtn{
        width: 128px;
        height: 52px;
        padding: 14px 32px;
        border-radius: 6px;
        font-weight: 500;
        border: none;
        background-color: #4CAF4F;
        color: #F5F7FA;
        font-size: 16px;
        line-height: 24px;
        letter-spacing: 0%;
        transition: background-color 0.4s ease;
    }
    .RegisterBtn:hover{
        background-color: #F5F7FA;
        color: #4CAF4F;
        box-shadow: 0px 0px 8px #4CAF4F;
    }
    .RegisterBtn:active{
        background-color: #4CAF4F;
        color: #F5F7FA;
    }
    .LearnBtn{
        width: 151px;
        height: 52px;
        padding: 14px 32px;
        border-radius: 6px;
        font-weight: 500;
        border: none;
        background-color: #4CAF4F;
        color: #F5F7FA;
        font-size: 16px;
        line-height: 24px;
        letter-spacing: 0%;
        transition: background-color 0.4s ease;
    }
    .LearnBtn:hover{
        background-color: #F5F7FA;
        color: #4CAF4F;
        box-shadow: 0px 0px 8px #4CAF4F;
    }
    .LearnBtn:active{
        background-color: #4CAF4F;
        color: #F5F7FA;
    }
</style>