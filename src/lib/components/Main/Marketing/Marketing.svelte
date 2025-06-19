<script>
    import MarketingCard from './MarketingCard/MarketingCard.svelte';
    import styles from './styles.module.css';
    import imageCardOne from '@assets/CardOne.png';
    import imageCardTwo from '@assets/CardTwo.png';
    import imageCardFree from '@assets/CardFree.png'

    const CardOne = {
        class:"CardOne",
        image:imageCardOne,
        title:"Creating Streamlined Safeguarding Processes with OneRen"
    };
    const CardTwo = {
        class:"CardTwo",
        image:imageCardTwo,
        title:"What are your safeguarding responsibilities and how can you manage them?"
    };
    const CardFree = {
        class:"CardFree",
        image:imageCardFree,
        title:"Revamping the Membership Model with Triathlon Australia"
    };
</script>
<section class = {styles.section}>
    <article class= {styles.title}> 
        <h2>Caring is the new marketing</h2>
        <p>The Nexcent blog is the best place to read about the latest membership 
            insights, trends and more. See who's joining the community, 
            read about how our community are increasing their membership income and lot's more.​
        </p>
    </article>
    <div class= {styles.CardBox}>
        <MarketingCard CardType = {CardOne}/>
        <MarketingCard CardType = {CardTwo}/>
        <MarketingCard CardType = {CardFree}/>
    </div>
</section>