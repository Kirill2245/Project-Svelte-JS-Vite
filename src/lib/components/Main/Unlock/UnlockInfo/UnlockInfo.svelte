<script>
    import Button from './../../../../common/Button/Button.svelte';
    import styles from './styles.module.css'
    const LearnBtn = {
        class:"LearnBtn",
        title:"Learn More"
    };
</script>
<div class= {styles.box}>
    <article class= {styles.title}>
        <h2>The unseen of spending three years at Pixelgrade</h2>
        <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed sit amet justo ipsum. Sed accumsan quam vitae est varius fringilla. 
            Pellentesque placerat vestibulum lorem sed porta. Nullam mattis tristique iaculis. 
            Nullam pulvinar sit amet risus pretium auctor. Etiam quis massa pulvinar, aliquam quam vitae, tempus sem. Donec elementum pulvinar odio.</p>
    </article>
    <Button buttonType = {LearnBtn}/>
</div>