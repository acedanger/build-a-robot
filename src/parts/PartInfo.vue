<template>
  <div>
    <h1>{{ part.title }}</h1>
    <div>
      {{ part.description }}
    </div>
  </div>
</template>

<script>
import parts from '../data/parts';

export default {
  name: 'PartInfo',
  computed: {
    part() {
      const { partType, id } = this.$route.params;

      return {
        title: 'Part Title',
        description: 'Part Description',
      };
    },
  },
};
</script>

<style>

</style>
