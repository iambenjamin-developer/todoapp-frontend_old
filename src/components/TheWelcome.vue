<script setup>
import WelcomeItem from './WelcomeItem.vue'
import DocumentationIcon from './icons/IconDocumentation.vue'
import ToolingIcon from './icons/IconTooling.vue'
import EcosystemIcon from './icons/IconEcosystem.vue'
import CommunityIcon from './icons/IconCommunity.vue'
import SupportIcon from './icons/IconSupport.vue'
</script>

<template>
  <WelcomeItem>
    <template #icon>
      <DocumentationIcon />
    </template>
    <template #heading>Documentation</template>
    <p>1 - Lorem ipsum dolor sit amet consectetur adipisicing elit. Delectus fugiat quos saepe corporis commodi incidunt autem officiis non, beatae eveniet. Deleniti asperiores reiciendis molestias distinctio dolorum consectetur quos libero consequuntur.</p>
  </WelcomeItem>

  <WelcomeItem>
    <template #icon>
      <ToolingIcon />
    </template>
    <template #heading>Tooling</template>

    <p>2 - Lorem ipsum, dolor sit amet consectetur adipisicing elit. Amet, harum deserunt nemo laboriosam fugit voluptas tenetur facilis accusantium, provident eligendi dolores placeat voluptatem et ipsam necessitatibus nostrum animi. Esse, provident.</p>
Este pasaporte
  </WelcomeItem>

  <WelcomeItem>
    <template #icon>
      <EcosystemIcon />
    </template>
    <template #heading>Ecosystem</template>
    
    <p> 3 - Lorem ipsum dolor sit amet, consectetur adipisicing elit. Necessitatibus, error reprehenderit? Debitis laudantium numquam, sequi dicta saepe unde ut provident doloremque quasi adipisci quod perspiciatis ad in odio dolore esse.</p>
  </WelcomeItem>

  <WelcomeItem>
    <template #icon>
      <CommunityIcon />
    </template>
    <template #heading>Community</template>
    <p> 4 - Lorem ipsum dolor, sit amet consectetur adipisicing elit. Vel, consequuntur perferendis libero doloribus placeat, quisquam quo eum ex, quidem blanditiis eius pariatur similique quibusdam nemo quis eligendi velit perspiciatis fuga.</p>
  </WelcomeItem>

  <WelcomeItem>
    <template #icon>
      <SupportIcon />
    </template>
    <template #heading>Support Vue</template>
 <p> 5 - Lorem ipsum, dolor sit amet consectetur adipisicing elit. Quos nisi dicta ad! Alias molestiae necessitatibus maxime nihil deleniti dolorum porro enim doloremque itaque laborum nobis expedita optio repellat, atque quaerat!</p>
  </WelcomeItem>
</template>
