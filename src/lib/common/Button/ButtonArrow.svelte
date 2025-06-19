<script>
    export let buttonType;
</script>
<button class = {buttonType.class}>{buttonType.title}<img src= {buttonType.image} alt=""></button>
<style>
    .readBtn{
        width: 285px;
        height: 44px;
        display: flex;
        font-size: 20px;
        line-height: 28px;
        font-weight: 600;
        color: #4CAF4F;
        padding: 8px 77px;
        border: none;
        border-radius: 2px;
        transition: background-color 0.4s ease;
    }
    .readBtn img{
        width: 24px;
        height: 24px;
        margin-left: 8px;
        margin-top: 2px;
    }
    .readBtn:hover{
        background-color: #E8F5E9;
    }
    .readBtn:active{
        box-shadow: 0px 0px 8px #4caf4f9c;
    }
</style>