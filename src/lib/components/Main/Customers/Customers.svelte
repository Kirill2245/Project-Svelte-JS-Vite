<script>
    import FrameLogo from './FrameLogo/FrameLogo.svelte';
    import FrameText from './FrameText/FrameText.svelte';
    import styles from './styles.module.css'
    import Image from '@assets/image 9.png'
    import { onMount } from 'svelte';
    
    const threshold = 0.35;
    onMount(() => {
        setTimeout(() => {
            const content = document.querySelectorAll('.content');
            content.forEach((box) => {
                const observer = new IntersectionObserver(
                    (entries) => {
                        entries.forEach((entry) => {
                            if (entry.isIntersecting) {
                                entry.target.classList.add('animation');
                            }
                            else{
                                entry.target.classList.remove('animation')
                            }
                        });
                    },
                    { threshold }
                );
                observer.observe(box);
            });
        }, 50);
    });
</script>
<div class= {styles.section}>
    <img src = {Image} alt = "" class= {styles.image}>
    <div class= "{styles.boxContent} content">
        <FrameText/>
        <FrameLogo/>
    </div>
</div>
<style>
    .content{
        opacity: 0;
        transform: translateX(-600px); 
        transition: opacity 0.9s ease, transform 0.9s ease; 
        
    }
    .content.animation {
        opacity: 1;
        transform: translateX(0); 
    }
</style>