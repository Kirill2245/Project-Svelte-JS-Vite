<script>
    import styles from './styles.module.css'
    export let cardType;

    import { onMount } from 'svelte';
    
    const threshold = 0.35;

    onMount(() => {
        
        setTimeout(() => {
            const cards = document.querySelectorAll('.card');
            console.log('Найдено элементов:', cards.length);  
            cards.forEach((card) => {
                const observer = new IntersectionObserver(
                    (entries) => {
                        entries.forEach((entry) => {
                            if (entry.isIntersecting) {
                                entry.target.classList.add('animate');
                            }
                            else{
                                entry.target.classList.remove('animate')
                            }
                        });
                    },
                    { threshold }
                );
                observer.observe(card);
            });
        }, 50);
    });
</script>
<div class= "{cardType.class} card" id = {styles.card}>
    <img src = {cardType.img} alt="">
    <article class= {styles.article}>
        <h3>{cardType.title}</h3>
        <aside>
            <p>{cardType.aside}</p>
        </aside>
    </article>
</div>
<style>
    .card{
        opacity: 0;
        transform: translateX(-300px);
        transition: all 0.6s ease-out;
    }
    .card.animate {
        opacity: 1;
        transform: translateX(0);
    }
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