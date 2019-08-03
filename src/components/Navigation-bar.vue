<template>
    <nav class="navbar navbar-expand-lg navbar-dark fixed-top" id="mainNav">
    <div class="container">
      <a class="navbar-brand js-scroll-trigger" href="#page-top">
        <img src="../assets/images/lgo.png">
      </a>
      <button class="navbar-toggler navbar-toggler-right" type="button" data-toggle="collapse" data-target="#navbarResponsive" aria-controls="navbarResponsive" aria-expanded="false" aria-label="Toggle navigation">
        Menu
        <i class="fas fa-bars"></i>
      </button>
      <div class="collapse navbar-collapse" id="navbarResponsive">
        <ul class="navbar-nav text-uppercase ml-auto" v-for="item in navItems" v-bind:key="item.title">
          <li class="nav-item">
            <a class="nav-link js-scroll-trigger" :href="`#${item.place}`">{{item.title}}</a>
          </li>
        </ul>
      </div>
    </div>
  </nav>
</template>

<script>
import Detail from '@/constants/detail';

export default {
  data() {
    return {
      navItems: [{
        title: 'Services',
        place: 'services'
      },
      {
        title: 'Portfolio',
        place: 'portfolio'
      },
      {
        title: 'Portfolio',
        place: 'portfolio'
      },
      {
        title: 'Services',
        place: 'services'
      }
      ]
    }

  }

}
</script>

<style>

</style>
