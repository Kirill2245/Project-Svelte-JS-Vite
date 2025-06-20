<script>
    import styles from './styles.module.css'
    import Button from '../../../common/Button/ButtonArrow.svelte';
    import Image from '@assets/RightWhite.svg'

    const ButtonGet = {
        class:"ButtonGet",
        title:"Get a Demo",
        image:Image
    };
</script>
<div class= {styles.section}>
    <h1 class= {styles.title}>Pellentesque suscipit fringilla libero eu.</h1>
    <Button buttonType = {ButtonGet}/>
</div>