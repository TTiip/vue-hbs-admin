<template>
  <a-dropdown>
    <div>
      <a-avatar :src="logoUrl" />
      <span class="ml-10px text-base text-black">Hongbusi</span>
    </div>

    <template #overlay>
      <a-menu>
        <a-menu-item key="lock">
          <span class="flex items-center">
            <lock-outlined class="mr-1" />
            <span>锁定屏幕</span>
          </span>
        </a-menu-item>
        <a-menu-item key="logout">
          <span class="flex items-center">
            <poweroff-outlined class="mr-1" />
            <span>退出登录</span>
          </span>
        </a-menu-item>
      </a-menu>
    </template>
  </a-dropdown>
</template>

<script setup lang="ts">
import { LockOutlined, PoweroffOutlined } from '@ant-design/icons-vue'
import logoUrl from '~/assets/logo.png'
</script>
