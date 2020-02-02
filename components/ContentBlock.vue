<template>
  <section
    class="c-ContentBlock"
    :class="sectionName"
    :style="{ backgroundColor: background, color: color }"
  >
    <div class="g-Container">
      <div class="c-ContentBlock_Text">
        <slot name="title" />
        <slot name="content" />
      </div>
      <div class="c-ContentBlock_SVG">
        <slot name="svg" />
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'ContentBlock',
  props: {
    sectionName: {
      type: String,
      default: ''
    },
    background: {
      type: String,
      default: '#fff'
    },
    color: {
      type: String,
      dafault: '#314259'
    }
  }
};
</script>

<style lang="scss" scoped>
.c-ContentBlock {
  padding: 15vh 0;
  position: relative;
}
.c-ContentBlock_Text {
  width: 50%;
}
h2 {
  text-transform: uppercase;
  font-size: 4.8rem;
  margin-top: 0;
  margin-bottom: 30px;
}
.c-ContentBlock_SVG {
  position: absolute;
  bottom: -5px;
  right: 12%;
}
</style>
