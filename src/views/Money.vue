<template>
  <Layout class-prefix="layout">
    <Number-pad />
    <Types :xxx="333" />
    <Notes/>
    <Tags :data-source="tags"/>
  </Layout>
</template>

<script>
import NumberPad from '@/components/Money/NumberPad.vue'
import Tags from '@/components/Money/Tags.vue'
import Notes from '@/components/Money/Notes.vue'
import Types from '@/components/Money/Types.vue'
export default {
  components: { NumberPad, Tags, Notes, Types },
  name: 'Money',
  data() {
    return {
      tags: ['衣', '食', '住', '行']
    }
  }
}
</script>

<style lang="scss">
.layout-content {
  display: flex;
  flex-direction: column-reverse;
}
</style>