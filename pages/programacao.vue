<template >
    <div >
   
    
          <programacaoSistema />
    
        
    </div>
</template>

<script setup>
import { onMounted } from 'vue';

definePageMeta({
  layout: 'dms',
});

const TitlePages = useTitlePagesStore()

onMounted(() => {
  TitlePages.setPageTitle('S2i - Sistema Integrado de Inspeção');
  TitlePages.setDrawerState(true)
});
</script>



