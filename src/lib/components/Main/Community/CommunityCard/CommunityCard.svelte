<script>
    import styles from './styles.module.css'
    export let cardType;
</script>
<div class= {cardType.class} id = {styles.div}>
    <img src = {cardType.img} alt="">
    <article class= {styles.article}>
        <h3>{cardType.title}</h3>
        <aside>
            <p>{cardType.aside}</p>
        </aside>
    </article>
</div>
<style>
    .MemberCard{
        margin-right:127px;
    }
    .MemberCard h3{
        width: 267px;
    }
    .MemberCard p{
        width: 251px;
        height: 60px;
    }
    .NationalCard{
        margin-right:127px;
    }   
    .NationalCard h3{
        width: 255px;
    }
    .NationalCard p{
        width: 240px;
        height: 80px;
    }  
    .ClubsCard h3{
        width: 222px;
    }
    .ClubsCard p{
        width: 251px;
        height: 60px;
    }
</style>