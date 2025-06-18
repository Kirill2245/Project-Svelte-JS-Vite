<script>
    import Button from './../../../../common/Button/Button.svelte';
    import styles from './styles.module.css';
    const RegisterBtn = {
        title:"Register",
        class:"RegisterBtn"
    };
</script>
<div class= {styles.box}>
    <div class= {styles.textBox}>
        <h1 class = {styles.title}>
            <span style="color: #4D4D4D;">Lessons and insights</span>
            <span style="color: #4CAF4F;">from 8 years</span>
        </h1>
        <p>Where to grow your business as a photographer: site or social media?</p>
    </div>
    <Button buttonType = {RegisterBtn}/>
</div>