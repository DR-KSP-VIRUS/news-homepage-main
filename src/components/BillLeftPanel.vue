<template>
    <figure id="mobile-image">
        <img src="/images/image-web-3-mobile.jpg" alt="image">
    </figure>
    <figure id="desktop-image">
        <img src="/images/image-web-3-desktop.jpg" alt="image">
    </figure>
    <div class="text">
        <div  class="title">
            <h1>The Bright Future of Web 3.0?</h1>
        </div>
        <div class="text-description">
            <p>
                We dive into the next evolution o the web that claims to put the power of the platforms back into the hands of the people.
                But is it really fulfulling its promise?
            </p>
            <div class="link-more">
                <a href="#">Read More</a>
            </div>
        </div>
    </div>
</template>


<style scoped>
    .title {
        font-family: 'Inter-ExtraBold';
        font-size: 23px;
        margin-right: 2rem;
    }

    .text-description p {
        color: var(--dark-grayish-blue);
        font-family: 'Inter-Regular';
        line-height: 2rem;
        font-size: 20px;
    }
    .link-more {
        margin-top: 2.5rem ;
    }
    .link-more a {
        background: var(--soft-red);
        color: var(--off-white);
        padding: 1rem 2.5rem;
        font-family: 'Inter-Bold';
        letter-spacing: 5px;
        text-transform: uppercase;
        transition: all 0.54s ease-in-out;
    }
    .link-more a:hover {
        background-color: var(--very-dark-blue);
    }
</style>