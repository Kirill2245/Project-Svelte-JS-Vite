<script>
    import Button from './../../../../common/Button/Button.svelte';
    import styles from './styles.module.css';
    import { onMount } from 'svelte';

    const RegisterBtn = {
        title:"Register",
        class:"RegisterBtn"
    };

    onMount(() => {
        const box = document.querySelectorAll('.box');
        box.forEach((element) => {
            setTimeout(() => {
                element.classList.add('visible');
            }, 300);
        });
    });
</script>
<div class= "box">
    <div class= {styles.textBox}>
        <h1 class = {styles.title}>
            <span style="color: #4D4D4D;">Lessons and insights</span>
            <span style="color: #4CAF4F;">from 8 years</span>
        </h1>
        <p>Where to grow your business as a photographer: site or social media?</p>
    </div>
    <Button buttonType = {RegisterBtn}/>
</div>
<style>
    .box{
        width: 657px;
        height: 276px;
        margin-right: 7.222%;
        opacity: 0;
        transform: translateX(-1100px);
        transition: opacity 0.9s ease, transform 0.9s ease;
    }

    .box.visible {
        opacity: 1;
        transform: translateX(0);
    }
    @media(max-width:1250px){
    .box{
        margin-right: 0;
    }
    }
</style>