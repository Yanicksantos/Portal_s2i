<template >
    <div >
      <v-container>
        <v-main>
          <tableSistemas />
        </v-main>
        
      </v-container>
        
    </div>
</template>

<script setup>
import { onMounted } from 'vue';

definePageMeta({
  layout: 'dms',
});

const TitlePages = useTitlePagesStore()

onMounted(() => {
  TitlePages.setPageTitle('MCI - Cadastro de Sistemas');
  TitlePages.setDrawerState(true)
});

</script>