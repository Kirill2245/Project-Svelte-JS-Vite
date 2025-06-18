<script>
    import styles from './styles.module.css';
    import elips1 from '@assets/Ellipse 5.svg';
    import elips2 from '@assets/Ellipse 6.svg';
    import elips3 from '@assets/Ellipse 7.svg';
    import illustration from '@assets/Illustration.png';
    import HeroInfo from './HeroInfo/HeroInfo.svelte';

</script>
<section class = {styles.section}>
    <div class= {styles.contain}>
        <HeroInfo/>
        <img src = {illustration} alt = "" class= {styles.image}> 
    </div>
    <div class= {styles.containImage}>
        <img src = {elips1} alt = "" >
        <img src = {elips2} alt = "">
        <img src = {elips3} alt = "">
    </div>
</section>