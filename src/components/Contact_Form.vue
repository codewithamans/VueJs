<template>
  <div class="text-[#201F23] text-[1.7rem] text-center font-bold">
    Fill up the form and our team will get back to you within 24 hours
  </div>
  <div class="grid lg:grid-cols-2 gap-8 mt-10">
    <Input
      placeholder="Name"
      icon="fa-user"
      v-model="name.value"
      :ref="name.ref"
      :is-danger="!!name.error"
      :error-message="name.error && name.error.message"
    />
    <Input
      placeholder="Email"
      icon="fa-user"
      v-model="email.value"
      :ref="email.ref"
      :is-danger="!!email.error"
      :error-message="email.error && email.error.message"
    />
    <Input
      placeholder="Phone"
      icon="fa-user"
      v-model="phone.value"
      :ref="phone.ref"
      :is-danger="!!phone.error"
      :error-message="phone.error && phone.error.message"
    />
    <Input
      placeholder="Subject"
      icon="fa-user"
      v-model="subject.value"
      :ref="subject.ref"
      :is-danger="!!subject.error"
      :error-message="subject.error && subject.error.message"
    />
  </div>
  <div class="mt-10">
    <input
      placeholder="Message (optional)"
      class="w-full h-[300px] border-2 border-[#01CB63] bg-[#F8F9FB]"
    />
  </div>
  <div class="flex justify-center">
    <button
      class="text-white w-[242px] italic flex justify-center mt-[55px] items-center bg-[#000] h-[70px] rounded-lg"
      @click="onSubmit"
    >
      Submit
    </button>
  </div>
</template>
<script>
import { defineComponent } from "vue";
import Input from "./Input.vue";
import { useForm } from "vue-hooks-form";

export default defineComponent({
  name: "Demo",
  components: {
    Input,
  },
  props: {
    modelValue: String,
  },
  setup() {
    const { useField, errors, values, handleSubmit } = useForm({
      defaultValues: {
        name: "Aman",
      },
    });
    const name = useField("name", {
      rule: { required: true },
    });
    const email = useField("email", {
      rule: { required: true },
    });
    const subject = useField("subject", {
      rule: { required: true },
    });
    const phone = useField("phone", {
      rule: {
        required: true,
        length: 10,
        min: 10,
      },
    });
    const message = useField("message", {
      rule: { required: true },
    });
    const onSubmit = (data) => console.log(data);
    return {
      name,
      phone,
      email,
      subject,
      message,

      onSubmit: handleSubmit(onSubmit),
      errors,
      values,
    };
  },
});
</script>
