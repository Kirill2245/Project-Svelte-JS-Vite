<script>
    import styles from './styles.module.css'
    import Logo1 from '@assets/Logo1.svg';
    import Logo2 from '@assets/Logo2.svg';
    import Logo3 from '@assets/Logo3.svg';
    import Logo4 from '@assets/Logo4.svg';
    import Logo5 from '@assets/Logo5.svg';
    import Logo6 from '@assets/Logo6.svg';
    import Logo7 from '@assets/Logo7.svg';
    let arrLogo = [Logo1,Logo2,Logo3,Logo4,Logo5,Logo6,Logo7]
</script>
<figure class= {styles.figure}>
    {#each arrLogo as logo,index}
        <img src={logo} alt="Logo" style:margin-left={index === 0 ? '0' : '136px'}>
    {/each}
</figure>
