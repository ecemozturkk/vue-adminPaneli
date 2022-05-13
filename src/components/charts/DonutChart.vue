<template>
  <div>
    <apexchart
      width="650"
      type="donut"
      :options="options"
      :series="series"
    ></apexchart>
  </div>
</template>

<script lang="ts" setup>
import { ref } from "vue";
const options = ref({
  labels: ['Plak', 'Tablo', 'Giyim', 'Fotoğraf Makinesi', 'Pikap'],
  
  title: {
          text: 'Kategorilere Göre Ürün Dağılımı',
          align: 'center',
          margin: 100,
          style: {
            fontSize: '20px',
            fontFamily: 'Verdana'
          },
        },
        
});
const series = ref([44, 55, 41, 17, 15]);
</script>