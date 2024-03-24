<template>
    <nav class="header-nav">
        <a class="logo" href="#">
            <img  src="/images/logo.svg" alt="icon">
        </a>
        <ul class="menu">
            <li class="nav-item">
               <a href="#">Home</a> 
            </li>
            <li class="nav-item">
                <a href="#">New</a>
            </li>
            <li class="nav-item"> 
                <a href="#">Popular</a>
            </li>
            <li class="nav-item"> 
                <a href="#">Trending</a>
            </li>
            <li class="nav-item"> 
                <a href="#">Categories</a>
            </li>
        </ul>
        <p class="mobile-menu"  href="#" @click="showSideNav">
            <img src="/images/icon-menu.svg" alt="icon">
        </p>
        <div :class="showNav ? 'side-show': 'hide-side-nav'">
          <ul class="side-nav">
            <img @click="closeSideNav" src="/images/icon-menu-close.svg" alt="">
            <li class="side-nav-item">
              <a href="#">Home</a> 
            </li>
            <li class="side-nav-item">
              <a href="#">New</a>
            </li>
            <li class="side-nav-item"> 
              <a href="#">Popular</a>
            </li>
            <li class="side-nav-item"> 
              <a href="#">Trending</a>
            </li>
            <li class="side-nav-item"> 
              <a href="#">Categories</a>
            </li>
          </ul>
        </div>
    </nav>
</template>

<script setup>

  import { ref } from 'vue';

  const showNav = ref(false);

  const showSideNav = () => {
    showNav.value = true;
  }
  
  const closeSideNav = () => {
    showNav.value = false;
  }
</script>

<style scoped>
    .header-nav {
      background: var(--off-white);
      display: flex;
      align-items: center;
      justify-content: flex-start;
      padding: .5rem 0;
      flex-wrap: wrap;
      width: 100%;
      position: relative;
      padding: 1.5rem;
    }
    .logo {
      margin-right: auto;
    }

    .nav-item {
      margin: 0 1rem;
      cursor: pointer;
      font-family: 'Inter-Regular';
      font-size: large;
    }
    .nav-item a {
      transition: all 0.54s ease-in-out;
      color: var(--very-dark-blue);
    }
    .nav-item a:hover {
      color: var(--soft-red);
    }

    .mobile-menu {
      cursor: pointer;
    }

    .side-nav-item {
      padding: 1rem;
      margin: 0 0 1rem 1rem;
      cursor: pointer;
      display: flex;
      place-items: center;
      font-family: 'Inter-Regular';
      font-size: large;
      transition: all 0.54s ease-in;
      width: 20rem;
    }

    .side-nav-item:hover {
      background: #f0efef;
    }

    .side-nav-item a {
      color: var(--very-dark-blue);
      transition: all 0.54s ease-in-out;
    }
    
    .side-show img {
      align-self: flex-end;
      position: absolute;
      top: 20px;
      right: 20px;
      cursor: pointer;
    }

    .hide-side-nav {
      display: none;
    }

    .side-nav {
      background: var(--off-white);
      position: absolute;
      height: 100%;
      right: 0;
      display: flex;
      flex-direction: column;
      padding-top: 5rem;
    }

</style>