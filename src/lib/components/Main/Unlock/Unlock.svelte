<script>
    import styles from './styles.module.css'
    import Image from '@assets/rafiki.png'
    import UnlockInfo from './UnlockInfo/UnlockInfo.svelte';
    export let UnlockProps;
</script>
<section class= {styles.section}>
    <img src = {UnlockProps.image} alt = "" class= {styles.image}>
    <UnlockInfo textUnlock = {UnlockProps}/>
</section>