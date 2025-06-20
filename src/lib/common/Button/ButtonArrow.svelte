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
    
    .ButtonGet{
        width: 178px;
        height: 52px;
        padding: 14px 32px;
        border: none;
        border-radius: 4px;
        background-color: #4CAF4F;
        color: #FFFFFF;
        font-size: 16px;
        line-height: 24px;
        display: flex;
        justify-content: center;
        align-items: center;
        transition: background-color 0.4s ease;
    }
    .ButtonGet img{
        width: 16px;
        height: 16px;
        /* margin: 4px 0px 4px 8px; */
        margin-left: 8px;
    }
    .ButtonGet:hover{
        background-color: #d1f5d4;
        color: #4CAF4F;
        box-shadow: 0px 0px 8px #4CAF4F;
    }
</style>