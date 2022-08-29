<template>
        <div class="Logo">
            <svg width="43" height="37" viewBox="0 0 43 37" fill="none" xmlns="http://www.w3.org/2000/svg">
                <path d="M21.3654 18.7836L7.71565 0H0V36.5718H9.2745L9.06491 16.3735L20.5401 32.485H22.1907L33.6659 16.3735L33.4563 36.5718H42.7308V0H35.0283L21.3654 18.7836Z" fill="white"/>
            </svg>
            <svg width="48" height="37" viewBox="0 0 48 37" fill="none" xmlns="http://www.w3.org/2000/svg">
                <path d="M19.7202 0L0.738876 36.5718H11.022L14.5851 29.1972H31.2085L20.6633 20.3948H18.8556L23.6893 10.8327L29.2959 22.2941L36.409 36.5718H47.5437L28.3135 0H19.7202Z" fill="white"/>
            </svg>
            <svg width="34" height="37" viewBox="0 0 34 37" fill="none" xmlns="http://www.w3.org/2000/svg">
                <path d="M10.4171 18.3383V8.80238H22.5342L33.0138 0H9.57871C7.69237 0 4.54847 0 2.55734 2.05651C0.566204 4.11302 0.513809 7.67588 0.513809 9.33943V18.3383V27.2847C0.513809 28.9483 0.513806 32.4064 2.55734 34.5677C4.60087 36.729 7.66617 36.6242 9.5525 36.6242H33.0531L22.5735 27.8087H10.4171V18.3383Z" fill="white"/>
            </svg>
            <svg class="point" width="23" height="37" viewBox="0 0 23 37" fill="none" xmlns="http://www.w3.org/2000/svg">
                <path d="M22.5456 0L0.656204 18.2859L22.5456 36.5849V0Z" fill="white"/>
            </svg>
            <svg width="43" height="37" viewBox="0 0 43 37" fill="none" xmlns="http://www.w3.org/2000/svg">
                <path d="M21.3654 18.7836L7.71565 0H0V36.5718H9.2745L9.06491 16.3735L20.5401 32.485H22.1907L33.6659 16.3735L33.4563 36.5718H42.7308V0H35.0283L21.3654 18.7836Z" fill="white"/>
            </svg>
            <svg width="48" height="37" viewBox="0 0 48 37" fill="none" xmlns="http://www.w3.org/2000/svg">
                <path d="M19.7202 0L0.738876 36.5718H11.022L14.5851 29.1972H31.2085L20.6633 20.3948H18.8556L23.6893 10.8327L29.2959 22.2941L36.409 36.5718H47.5437L28.3135 0H19.7202Z" fill="white"/>
            </svg>
            <p class="LogoText">Автотовары онлайн</p>
        </div>
</template>

<script>
export default {
    name: 'LogoMagma',
}
</script>

<style scoped>

.Logo {
    /* width: 238px;
    height: 57px; */
}

.point {
    margin-left: -22px;
}

.Logo svg{
    margin-right: 4px;
    object-fit: contain;
}

.LogoText {
    margin-top: 5px;
    font-size: 10px;
    line-height: 10px;
    letter-spacing: 0.47rem;
    text-transform: uppercase;
    text-align: center;
}

</style>