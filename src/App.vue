<template>
  <img alt="Vue logo" src="./assets/logo.png" />
  {{ value }}
  <section class="ass">
    <BaseCurrencyField
      label="Currency Field"
      v-model="value"
      horizontal
      expanded
    />
  </section>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import { BaseCurrencyField } from "peerstreet-design-library-vue3";

export default defineComponent({
  name: "App",
  data() {
    return { value: null };
  },
  components: {
    BaseCurrencyField,
  },
});
</script>

<style>
.ass {
  text-align: left;
  width: 50%;
}
</style>
