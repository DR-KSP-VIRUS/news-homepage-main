<template>
    <picture >
        <img id="mobile-image" src="/images/image-web-3-mobile.jpg" alt="mobile-image">
        <img id="desktop-image" src="/images/image-web-3-desktop.jpg" alt="desktop-image">
    </picture>
    <div class="text">
        <h1 class="title">The Bright Future of Web 3.0?</h1>
        <div class="text-description">
            <p>
                We dive into the next evolution o the web that claims to put the power of the platforms back into the hands of the people.
                But is it really fulfulling its promise?
            </p>
            <div class="read-more">
                <a href="#">Read More</a>
            </div>
        </div>
    </div>
</template>


<style scoped>
    .title {
        font-family: 'Inter-ExtraBold';
        font-size: 3.5rem;
        margin-right: 2rem;
        margin-bottom: 1rem;
    }

    .text-description p {
        color: var(--dark-grayish-blue);
        font-family: 'Inter-Regular';
        line-height: 2rem;
        font-size: 1.19rem;
        padding-bottom: 1rem;
    }
    .read-more {
        margin-top: .5rem ;
    }
    .read-more a {
        background: var(--soft-red);
        color: var(--off-white);
        padding: .7rem 2.5rem;
        font-family: 'Inter-Bold';
        letter-spacing: .2rem;
        text-transform: uppercase;
        transition: all 0.54s ease-in-out;
    }
    .read-more a:hover {
        background-color: var(--very-dark-blue);
    }
</style>