<script setup lang="ts">

import WhatsappIcon from "@/icons/WhatsappIcon.vue";
import { Button } from "@/components/ui/button";
import { Instagram } from "lucide-vue-next";
import { Avatar, AvatarFallback, AvatarImage, } from "@/components/ui/avatar"
</script>

<template>
  <section class="intro">
    <div
      class="grid place-items-center lg:max-w-screen-xl gap-8 mx-auto py-20 md:py-32"
    >
      <div class="text-center space-y-8">

        <Avatar class="size-60">
          <AvatarImage src="https://i.ibb.co/rRxZd2G9/Screenshot-2025-03-31-020947.png" alt="@shadcn" />
          <AvatarFallback>CN</AvatarFallback>
        </Avatar>
        <!-- <Badge
          variant="outline"
          class="text-sm py-2"
        >
          <span class="mr-2 text-primary">
            <Badge>Atendimento</Badge>
          </span>
          <span> Especial </span>
        </Badge> -->

        <div
          class="max-w-screen-md mx-auto text-center text-5xl md:text-6xl font-bold"
        >
          <h1>
            Ygor Diniz
            <span
              class="text-transparent bg-gradient-to-r from-[#D247BF] to-primary bg-clip-text"
              >Psicologia
            </span>
          </h1>
        </div>

        <p class="max-w-screen-sm mx-auto text-xl text-muted-foreground">
          Um texto bem bonito
        </p>

        <div class="space-y-4 md:space-y-0 md:space-x-4">
          <Button class="w-5/6 md:w-1/4 font-bold">
            <a href="https://www.instagram.com/ygordiniz.psi" target="_blank">
              <WhatsappIcon class="size-5 mr-2"/>
            </a>
            <a href="https://www.instagram.com/ygordiniz.psi" target="_blank">
              Whatsapp
            </a>
          </Button>

          <Button as-child variant="secondary" class="w-5/6 md:w-1/4 font-bold">
            <a href="https://www.instagram.com/ygordiniz.psi" target="_blank">
                <Instagram class="size-5 mr-2"/>
                Instagram
            </a>
          </Button>
        </div>
      </div>

    </div>
  </section>
</template>

<style scoped>
.img-shadow-animation {
  animation-name: img-shadow-animation;
  animation-iteration-count: infinite;
  animation-duration: 2s;
  animation-timing-function: linear;
  animation-direction: alternate;
}

.img-border-animation {
  animation-name: img-border-animation;
  animation-iteration-count: infinite;
  animation-duration: 2s;
  animation-timing-function: linear;
  animation-direction: alternate;
}

@keyframes img-shadow-animation {
  from {
    opacity: 0.5;
    transform: translateY(30px);
  }

  to {
    opacity: 1;
    transform: translateY(0px);
  }
}
@keyframes img-border-animation {
  from {
    @apply border-t-primary/10;
  }

  to {
    @apply border-t-primary/60;
  }
}
</style>
