<template>
  <card>
    <a class="main-link" href="https://shshacks.io" target="_blank">
      <img class="logo" src="@/assets/occasions/shsHacks.png">
      <div class="register">
        Stevenson's free-to-attend hackathon is happening this weekend. <br><span class="color">Register Now!</span>&nbsp;
        <font-awesome-icon :icon="faArrowUpRightFromSquare" class="link-icon" />
      </div>
    </a>
  </card>
</template>

<script>
import Card from '@/components/Card.vue';
import { faArrowUpRightFromSquare } from '@fortawesome/free-solid-svg-icons';

export default {
  components: { Card },
  data() {
    return {
      faArrowUpRightFromSquare,
    };
  },
};
</script>

<style lang="sass" scoped>
.main-link
  display: flex
  align-items: center
  text-decoration: none
  justify-content: center
  flex-direction: column
  color: var(--primary)
  .logo
    height: 150px
    margin: 10px
    background: white
    border-radius: 15px
  .register
    font-size: .85em
    text-align: left
    padding-bottom: 10px
    margin: 0 20px
    line-height: 1.6em
    text-align: center
    .color
      color: var(--color)
      font-weight: bold

    .link-icon
      font-size: 1.1em
      color: var(--color)

</style>
