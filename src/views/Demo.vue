<template>
  <div class="Demo px-5">
    <h1>Demo Task</h1>
    <h3>Task description</h3>
    <p>
      Lorem ipsum dolor sit amet consectetur adipisicing elit. Eos minima omnis
      eum ab non maiores, facere quibusdam voluptates deserunt nam dicta
      similique sapiente ipsum necessitatibus fuga laborum velit nemo maxime!
    </p>
    <p>
      Lorem ipsum dolor sit amet consectetur adipisicing elit. Esse hic eligendi
      accusamus fugit veniam impedit tenetur id veritatis, dolor reiciendis
      exercitationem est, rerum deleniti eaque aut labore, minus laboriosam
      soluta?
    </p>
    <div class="ml-2 d-flex"><grid-image /></div>
  </div>
</template>
<script>
import gridImage from "../components/gridImage.vue";
export default {
  name: "Demo",
  components: { gridImage },

  data() {
    return {};
  },
};
</script>
