<script>
    import Achievements from './Achievements/Achievements.svelte';
    import Clients from './Clients/Clients.svelte';
    import Community from './Community/Community.svelte';
    import Hero from './HeroSection/Hero.svelte';
    import styles from './styles.module.css'
    import Unlock from './Unlock/Unlock.svelte';
    
</script>
<main class={styles.main}>
    <Hero/>
    <Clients/>
    <Community/>
    <Unlock/>
    <Achievements/>
</main>