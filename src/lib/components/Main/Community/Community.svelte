<script>
    import CommunityCard from './CommunityCard/CommunityCard.svelte';
    import CommunityTitle from './CommunityTitle/CommunityTitle.svelte';
    import member from '@assets/member.svg'
    import national from '@assets/national.svg'
    import clubs from '@assets/clubs.svg'
    import styles from './styles.module.css'
    const MemberCard = {
        class:"MemberCard",
        title:"Membership Organisations",
        img:member,
        aside:"Our membership management software provides full automation of membership renewals and payments"
    }
    const NationalCard = {
        class:"NationalCard",
        title:"National Associations",
        img:national,
        aside:"Our membership management software provides full automation of membership renewals and payments"
    }
    const ClubsCard = {
        class:"ClubsCard",
        title:"Clubs And Groups",
        img:clubs,
        aside:"Our membership management software provides full automation of membership renewals and payments"
    }
    
</script>
<section class={styles.section}>
    <CommunityTitle/>
    <div class= {styles.cardBox}>
        <CommunityCard cardType = {MemberCard}/>
        <CommunityCard cardType = {NationalCard}/>
        <CommunityCard cardType = {ClubsCard}/>
    </div>
</section>