<script>
    import styles from './styles.module.css'
    import Logo from './Logo/Logo.svelte';
    import NavigationMenu from './NavigationMenu/NavigationMenu.svelte';
    import Button from './../../common/Button/Button.svelte';

    const logBtn = {
        title:"Login",
        class:"LoginBtn"
    }
    const SignBtn = {
        title:"Sign up",
        class:"SignBtn"
    }
</script>

<header class = {styles.header}>
    <Logo/>
    <NavigationMenu/>
    <Button buttonType = {logBtn}/>
    <Button buttonType = {SignBtn}/>
</header>