<script>
    import Button from './../../../../common/Button/Button.svelte';
    import styles from './styles.module.css'
    const LearnBtn = {
        class:"LearnBtn",
        title:"Learn More"
    };
    export let textUnlock;
</script>
<div class= {styles.box} id = {textUnlock.class}>
    <article class= {styles.title}>
        <h2>{textUnlock.title}</h2>
        <p>{textUnlock.text}</p>
    </article>
    <Button buttonType = {LearnBtn}/>
</div>
<style>
    #UnlockOne p{
        height: 80px;
    }
    #UnlockOne{
        height: 268px;
        margin: 82.5px 0 82.5px 49px;
    }
    #UnlockOne article{
        height: 184px;
    }
    #UnlockTwo p{
        height: 120px;
    }
    #UnlockTwo article{
        height: 224px;
    }
    #UnlockTwo{
        height: 308px;
        margin: 62.7px 0 62.7px 49px;
    }
</style>