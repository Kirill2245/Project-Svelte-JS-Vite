<script>
    import ButtonArrow from './../../../../common/Button/ButtonArrow.svelte';
    import styles from './styles.module.css';
    import ImageBtn from '@assets/Right.svg';
    export let CardType;

    const readBtn = {
        image:ImageBtn,
        title:"Readmore",
        class:"readBtn"
    };
</script>
<div class= {styles.Card}>
    <img src = {CardType.image} alt="">
    <div class= {styles.frame}>
        <h4>{CardType.title}</h4>
        <ButtonArrow buttonType = {readBtn}/>
    </div>
</div>