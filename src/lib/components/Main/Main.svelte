<script>
    import Clients from './Clients/Clients.svelte';
    import Community from './Community/Community.svelte';
    import Hero from './HeroSection/Hero.svelte';
    import styles from './styles.module.css'
    
</script>
<main class={styles.main}>
    <Hero/>
    <Clients/>
    <Community/>
</main>