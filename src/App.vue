<template>

  <n-config-provider :theme="darkTheme">
    <n-layout position="absolute" class="capys">
      <n-layout-header style="height: 64px; padding: 24px" bordered>
        颐和园路
      </n-layout-header>
      <n-layout position="absolute" style="top: 64px;padding: 8px;" :native-scrollbar="false">
        <div class="base">
          <router-view></router-view>
        </div>
      </n-layout>
    </n-layout>
  </n-config-provider>


</template>

<script setup lang="ts">
import { darkTheme } from "naive-ui";
</script>