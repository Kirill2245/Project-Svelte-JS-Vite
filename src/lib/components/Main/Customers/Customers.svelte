<script>
    import FrameLogo from './FrameLogo/FrameLogo.svelte';
    import FrameText from './FrameText/FrameText.svelte';
    import styles from './styles.module.css'
    import Image from '@assets/image 9.png'
</script>
<div class= {styles.section}>
    <img src = {Image} alt = "" class= {styles.image}>
    <div class= {styles.boxContent}>
        <FrameText/>
        <FrameLogo/>
    </div>
</div>