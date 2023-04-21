<template>
  <div class="field">
    <label class="label">{{ label }}</label>
    <div class="control has-icons-left has-icons-right">
      <input
        class="py-3 w-full border-r-0 border-l-0 border-t-0 border-2 border-b-[#01CB63] bg-[#F8F9FB]"
        type="text"
        :value="modelValue"
        @input="(e) => $emit('update:modelValue', e.target.value)"
        v-bind="$attrs"
      />
      <p class="text-red-600 capitalize mt-1">{{ errorMessage }}</p>
    </div>
  </div>
</template>

<script>
import { defineComponent } from "vue";

export default defineComponent({
  name: "Input",
  components: {},
  props: {
    modelValue: String,
    label: String,
    icon: String,
    errorMessage: String,
    isDanger: Boolean,
  },
});
</script>
