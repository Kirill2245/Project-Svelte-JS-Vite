<script>
    import AchievementsCard from './AchievementsCard/AchievementsCard.svelte';
    import styles from './styles.module.css'
    import card1 from '@assets/card1.svg'
    import card2 from '@assets/card2.png'
    import card3 from '@assets/card3.svg'
    import card4 from '@assets/card4.svg'
    const Card1 = {
        class:"Card1",
        title:"2,245,341",
        text:"Members",
        image:card1
    }
    const Card2 = {
        class:"Card2",
        title:"46,328",
        text:"Clubs",
        image:card2
    }
    const Card3 = {
        class:"Card3",
        title:"828,867",
        text:"Event Bookings",
        image:card3
    }
    const Card4 = {
        class:"Card4",
        title:"1,926,436",
        text:"Payments",
        image:card4
    }
</script>
<section class= {styles.section}>
    <article class= {styles.article}>
        <h2 class= {styles.title}>
            <span style="color: #4D4D4D;">Helping a local</span>
            <span style="color: #4CAF4F;">business reinvent itself</span>
        </h2>
        <p>We reached here with our hard work and dedication</p>
    </article>
    <div class= {styles.boxCard}>
        <AchievementsCard typeCard = {Card1}/>
        <AchievementsCard typeCard = {Card2}/>
        <AchievementsCard typeCard = {Card3}/>
        <AchievementsCard typeCard = {Card4}/>
    </div>
</section>