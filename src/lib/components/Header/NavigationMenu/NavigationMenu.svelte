<script>
    import styles from './styles.module.css'

    const links = [
        { path: '/', title: 'Home' },
        { path: '/', title: 'Service' },
        { path: '/', title: 'Feature' },
        { path: '/', title: 'Product' },
        { path: '/', title: 'Testimonial' },
        { path: '/', title: 'FAQ' },
    ];
</script>
<nav class = {styles.nav}>
    <ul class = {styles.ul}>
        {#each links as link, index}
            <li class= {styles.li}>
                <a 
                    href={link.path} 
                    class = {styles.a}
                    style:margin-left={index === 0 ? '0' : '50px'}
                >
                    {link.title}
                </a>
            </li>
        {/each}
    </ul>
</nav>