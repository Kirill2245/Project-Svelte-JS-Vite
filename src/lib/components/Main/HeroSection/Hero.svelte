<script>
    import styles from './styles.module.css';
    import elips1 from '@assets/Ellipse 5.svg';
    import elips2 from '@assets/Ellipse 6.svg';
    import elips3 from '@assets/Ellipse 7.svg';
    import illustration from '@assets/Illustration.png';
    import HeroInfo from './HeroInfo/HeroInfo.svelte';
    import { onMount } from 'svelte';

    onMount(() => {
        const images = document.querySelectorAll('.image');
        images.forEach((element) => {
            setTimeout(() => {
                element.classList.add('visible');
            }, 320);
        });
    });
</script>
<section class = {styles.section}>
    <div class= {styles.contain}>
        <HeroInfo/>
        <img src = {illustration} alt = "" class= "image"> 
    </div>
    <div class= {styles.containImage}>
        <img src = {elips1} alt = "" >
        <img src = {elips2} alt = "">
        <img src = {elips3} alt = "">
    </div>
</section>
<style>
    .image {
        width: 391px;
        height: 407px;
        margin-top: 96px;
        margin-bottom: 55px;
        opacity: 0;
        transform: translateX(1800px);
        transition: opacity 0.9s ease, transform 0.9s ease;
    }

    .image.visible {
        opacity: 1;
        transform: translateX(0);
    }
</style>