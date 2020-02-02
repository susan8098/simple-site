<template>
  <section class="c-StatsBlock">
    <div class="g-Container">
      <p>
        <slot />
      </p>
    </div>
  </section>
</template>

<script>
export default {
  name: 'StatsBlock'
};
</script>

<style lang="scss" scoped>
.c-StatsBlock {
  text-align: center;
  padding: 15vh 0;
}
p {
  font-size: 4.6rem;
  font-weight: 600;
  line-height: 1.3;
}
</style>
