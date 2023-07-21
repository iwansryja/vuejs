<script setup>
import { RouterLink, RouterView } from 'vue-router'
import BottomNavItem from './components/BottomNavItem.vue'
</script>

<template>
  <!-- loader -->
  <!-- <div id="loader">
        <img src="assets/img/loading-icon.png" alt="icon" class="loading-icon">
    </div> -->
    <!-- * loader -->

    <!-- App Header -->
    <div class="appHeader">
        <div class="left">
            <a href="#" class="headerButton goBack">
                <ion-icon name="chevron-back-outline"></ion-icon>
            </a>
        </div>
        <div class="pageTitle">
            About
        </div>
        <div class="right">
            <!-- <a href="app-notifications.html" class="headerButton">
                <ion-icon class="icon" name="notifications-outline"></ion-icon>
                <span class="badge badge-danger">4</span>
            </a> -->
        </div>
    </div>
    <!-- * App Header -->

    <!-- App Capsule -->
    <div id="appCapsule">
      <RouterView />
    </div>
    <!-- * App Capsule -->


    <!-- App Bottom Menu -->
    <div class="appBottomMenu">

        <RouterLink to="/" class="item">
          <BottomNavItem>
            <template #icon>
              <ion-icon name="pie-chart-outline"></ion-icon>
            </template>
            <template #title>Home</template>
          </BottomNavItem>
        </RouterLink>
        
        <RouterLink to="/home" class="item">
          <BottomNavItem>
            <template #icon>
              <ion-icon name="document-text-outline"></ion-icon>
            </template>
            <template #title>Home</template>
          </BottomNavItem>
        </RouterLink>

        <RouterLink to="/about" class="item">
          <BottomNavItem>
            <template #icon>
              <ion-icon name="settings-outline"></ion-icon>
            </template>
            <template #title>Home</template>
          </BottomNavItem>
        </RouterLink>

    </div>
</template>

<style scoped>
</style>
