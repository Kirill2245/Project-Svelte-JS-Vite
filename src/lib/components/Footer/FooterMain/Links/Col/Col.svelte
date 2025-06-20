<script>
    import styles from './styles.module.css'

    export let typeCol
</script>
<div class= {styles.section}>
    <h4 class= {styles.title}>{typeCol.title}</h4>
    <div class= {styles.list}>
        {#each typeCol.arrItem as item}
            <p>{item}</p>
        {/each}
    </div>
</div>