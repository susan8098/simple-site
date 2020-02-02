<template>
  <header class="c-Hero">
    <Logo />
    <h1>
      Let's help you <br />
      <a href="#">buy</a>, <a href="#">sell</a> and <a href="#">invest</a>.
    </h1>
    <div class="triangle"></div>
  </header>
</template>

<script>
import Logo from '@/components/Logo.vue';
export default {
  name: 'Hero',
  components: { Logo }
};
</script>

<style lang="scss" scoped>
.c-Hero {
  height: 100vh;
  background-image: url('/hero-bg.png');
  background-size: cover;
  text-align: center;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  align-items: center;

  .c-Logo {
    margin-top: 50px;
  }
}
h1 {
  color: white;
  margin-top: 0;
  margin-bottom: 80px;
  line-height: 1.4;
  letter-spacing: 0.8px;
  a {
    color: white;
    display: inline-block;
    text-decoration: none;
    position: relative;

    &:after {
      content: '';
      width: 100%;
      height: 2px;
      background: white;
      position: absolute;
      bottom: 3px;
      left: 0;
    }
  }
}
.triangle {
  width: 0;
  height: 0;
  border-style: solid;
  border-width: 20px 15px 0 15px;
  border-color: #ffffff transparent transparent transparent;
  margin-bottom: 20px;
}
</style>
