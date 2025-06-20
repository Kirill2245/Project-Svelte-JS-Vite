<script>
    import Col from './Col/Col.svelte';
    import styles from './styles.module.css';

    const Company = {
        title:"Company",
        arrItem:["About us", "Blog", "Contact us", "Pricing", "Testimonials"]
    };
    const Support = {
        title:"Support",
        arrItem:["Help center", "Terms of service", "Legal", "Privacy policy", "Status"]
    }

</script>
<div class= {styles.section}>
    <Col typeCol = {Company}/>
    <Col typeCol = {Support}/>
    <div class= {styles.inputBox}>
        <h4>Stay up to date</h4>
        <input placeholder="Your email address" type="email" class= {styles.input}>
    </div>
</div>