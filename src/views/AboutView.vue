<template>
  <div><BasicArea :option="option"></BasicArea>
    </div>
</template>

<script>
import BasicArea from "@/components/BasicArea.vue";
import option from "../mock/index";

export default {
  name: "AboutView",
  components: {
    BasicArea,
  },
  data() {
    return {
      option:option
    };
  },
  mounted(){
    console.log("这是view中的this")
    console.log(this)
  }
};
</script>
