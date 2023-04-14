<script>
import ComicsCard from "./ComicsCard.vue";
import comics from "../data/dc-comics.json";
export default {
  name: "MainComics",
  components: {
    ComicsCard,
  },
  data() {
    return {
      comics: comics,
    };
  },
};
</script>

<template>
  <div class="main_comics">
    <div class="comics_container">
      <div class="section_title">
        <h3>CURRENT SERIES</h3>
      </div>
      <!-- /.section_title -->
      <div class="row row-cols-lg-6">
        <ComicsCard
          v-for="comic in comics"
          :img="comic.thumb"
          :title="comic.series"
        />
      </div>
      <!-- /.row -->
      <button type="button" class="btn btn-primary rounded-0 d-block px-5">LOAD MORE</button>
    </div>
    <!-- /.comics_container -->
  </div>
</template>

<style lang="scss" scoped></style>
