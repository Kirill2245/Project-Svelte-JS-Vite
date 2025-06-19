<script>
    import Achievements from './Achievements/Achievements.svelte';
    import Clients from './Clients/Clients.svelte';
    import Community from './Community/Community.svelte';
    import Hero from './HeroSection/Hero.svelte';
    import styles from './styles.module.css'
    import Unlock from './Unlock/Unlock.svelte';
    import ImageUnlockOne from '@assets/rafiki.png'
    import ImageUnlockTwo from '@assets/pana.png'
    import Customers from './Customers/Customers.svelte';

    const UnlockOne = {
        class:"UnlockOne",
        image:ImageUnlockOne,
        title:"The unseen of spending three years at Pixelgrade",
        text:"Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed sit amet justo ipsum. Sed accumsan quam vitae est varius fringilla. Pellentesque placerat vestibulum lorem sed porta. Nullam mattis tristique iaculis. Nullam pulvinar sit amet risus pretium auctor. Etiam quis massa pulvinar, aliquam quam vitae, tempus sem. Donec elementum pulvinar odio."
    }
    const UnlockTwo = {
        class:"UnlockTwo",
        image:ImageUnlockTwo,
        title:"How to design your site footer like we did",
        text:"Donec a eros justo. Fusce egestas tristique ultrices. Nam tempor, augue nec tincidunt molestie, massa nunc varius arcu, at scelerisque elit erat a magna. Donec quis erat at libero ultrices mollis. In hac habitasse platea dictumst. Vivamus vehicula leo dui, at porta nisi facilisis finibus. In euismod augue vitae nisi ultricies, non aliquet urna tincidunt. Integer in nisi eget nulla commodo faucibus efficitur quis massa. Praesent felis est, finibus et nisi ac, hendrerit venenatis libero. Donec consectetur faucibus ipsum id gravida."
    }
    
</script>
<main class={styles.main}>
    <Hero/>
    <Clients/>
    <Community/>
    <Unlock UnlockProps = {UnlockOne}/>
    <Achievements/>
    <Unlock UnlockProps = {UnlockTwo}/>
    <Customers/>
</main>