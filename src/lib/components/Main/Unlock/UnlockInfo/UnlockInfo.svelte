<script>
    import Button from './../../../../common/Button/Button.svelte';
    import styles from './styles.module.css'

    const LearnBtn = {
        class:"LearnBtn",
        title:"Learn More"
    };

    export let textUnlock;

    import { onMount } from 'svelte';
    
    const threshold = 0.35;
    onMount(() => {
        setTimeout(() => {
            const title = document.querySelectorAll('.line');
            title.forEach((line) => {
                const observer = new IntersectionObserver(
                    (entries) => {
                        entries.forEach((entry) => {
                            if (entry.isIntersecting) {
                                entry.target.classList.remove('animationclose')
                                entry.target.classList.add('animation');
                                setTimeout(() => {
                                    entry.target.classList.remove('animation')
                                    entry.target.classList.add('animationclose');
                                },800)
                            }
                            else{
                                entry.target.classList.remove('animation')
                                entry.target.classList.remove('animationclose')
                            }
                        });
                    },
                    { threshold }
                );
                observer.observe(line);
            });
        }, 50);
    });
</script>
<div class= {styles.box} id = {textUnlock.class}>
    <article class= {styles.title}>
        <div class= "contain">
            <h2>{textUnlock.title}</h2>
            <div class= "line"></div>
        </div>
        <p>{textUnlock.text}</p>
    </article>
    <Button buttonType = {LearnBtn}/>
</div>
<style>
    .contain {
        position: relative;
    }
    .line {
        position: absolute;
        bottom: 0;
        left: 0;
        width: 100%;
        height: 3px;
        background-color: #4CAF4F; 
        transform: scaleX(0); 
        transform-origin: left center;
        transition: transform 0.9s ease; 
    }
    .line.animation{
        transform: scaleX(1); 
    }
    .line.animationclose{
        transform: scaleX(0); 
        transform-origin: right center;
    }
    #UnlockOne p{
        height: 80px;
    }
    #UnlockOne{
        height: 268px;
        margin: 82.5px 0 82.5px 49px;
    }
    #UnlockOne article{
        height: 184px;
    }
    #UnlockTwo p{
        height: 120px;
    }
    #UnlockTwo article{
        height: 224px;
    }
    #UnlockTwo{
        height: 308px;
        margin: 62.7px 0 62.7px 49px;
    }
    @media(max-width:1150px){
        #UnlockOne{
            margin: 82.5px 0 ;
        }
        #UnlockTwo{
            margin: 62.7px 0 ;
        }
    }
</style>