<template>
  <Layout class-prefix="layout">
    <Number-pad/>
    <Types :xxx="333"/>
    <Notes/>
    <Tags/>

  </Layout>
</template>

<script lang="ts">
import NumberPad from '@/components/Money/NumberPad.vue'
import Tags from '@/components/Money/Tags.vue'
import Notes from '@/components/Money/Notes.vue'
import Types from '@/components/Money/Types.vue'
export default {
  components: { NumberPad, Tags, Notes, Types },
  name: 'Money'
}
</script>

<style lang="scss">
.layout-content {
  display: flex;
  flex-direction: column-reverse;
}
</style>