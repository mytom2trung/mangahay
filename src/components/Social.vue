<template>
  <div class="flex items-center justify-center">
    <q-btn
      v-for="social in socials"
      :key="social.href"
      :href="social.href"
      target="_blank"
      round
      unelevated
    >
      <component :is="social.icon" class="size-1.5em" />
    </q-btn>
  </div>
</template>

<script lang="ts" setup>
import LogoFacebook from "~icons/logos/facebook"
import LogosTelegram from "~icons/logos/telegram"

const socials = [
  // { icon: LogosTwitter, href: "https://twitter.com/" },
  // { icon: LogosGithub, href: "https://github.com/" },
  { icon: LogoFacebook, href: "https://www.facebook.com/animehay.fanpage" },
  { icon: LogosTelegram, href: "https://t.me/+B-Vh8f4e55VhMzg1" }
]
</script>
