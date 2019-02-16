<template>
  <div id="NotFound">
    <section class="c-empty">
      <div class="c-empty__wrap">
        <img :src="PlaceholderImg" alt="" class="c-empty__img">
        <h3 class="c-empty__title">暂无数据</h3>
      </div>
    </section>
  </div>

</template>

<script>
  import { mapActions, mapState, mapGetters } from "vuex";
  import PlaceholderImg from "../../images/placeholder.png";

  export default {
    name: "NotFound",
    data() {
      return {
        PlaceholderImg
      };
    },
    methods: {},
    computed: {},
    created() {
    }
  };
</script>

<style scoped lang="scss">
  @import "../../style/mixin";

  #NotFound {
    min-height: 100px;
    .c-empty {
      overflow: hidden;
      padding-bottom: 60px;
      &__wrap {
        margin-top: 100px;
        @include alignCenter;
        flex-direction: column;
      }
      &__img {
        width: 300px;
        height: 210px;
      }
      &__title {
        margin-top: 35px;
        font-size: 18px;
        color: rgba(153, 153, 153, 1);
      }
    }
  }
</style>
