<script>
    import styles from './styles.module.css'
    import Image from '@assets/rafiki.png'
    import UnlockInfo from './UnlockInfo/UnlockInfo.svelte';
</script>
<section class= {styles.section}>
    <img src = {Image} alt = "" class= {styles.image}>
    <UnlockInfo/>
</section>