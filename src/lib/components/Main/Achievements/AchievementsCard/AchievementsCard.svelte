<script>
    import styles from './styles.module.css'
    export let typeCard
</script>
<div class= {typeCard.class} id = {styles.Card}>
    <img src = {typeCard.image} alt = "">
    <article>
        <h3>{typeCard.title}</h3>
        <p>{typeCard.text}</p>
    </article>
</div>
<style>
    .Card1{
        margin-right: 30px;
    }
    .Card3{
        margin-right: 30px;
    }

</style>