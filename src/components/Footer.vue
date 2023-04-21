<template>
  <div class="w-full mt-32">
    <div class="italic text-[#01CB63] text-center font-semibold text-xl">
      Contact Us
    </div>
    <div class="text-black mt-4 text-4xl text-center font-bold">
      Reach Out with any
    </div>
    <div class="text-black mt-4 text-4xl text-center font-bold">
      question you have
    </div>
    <div class="mt-20 bg-[#F8F9FB] flex justify-center">
      <div class="w-4/5">
        <div class="grid lg:grid-cols-2">
          <div class="mt-20">
            <div class="text-[#201F23] text-4xl font-bold">
              Contact Information
            </div>
            <div class="flex mt-16 space-x-4">
              <div>
                <img src="@/assets/images/mail.svg" alt="" srcset="" />
              </div>
              <div class="text-[#201F23] mt-10 text-xl font-bold">
                contact@coursepro.com
              </div>
            </div>
            <div class="flex mt-6 space-x-4">
              <div>
                <img src="@/assets/images/phone.svg" alt="" srcset="" />
              </div>
              <div class="text-[#201F23] mt-10 text-xl font-bold">
                1800-562-895, 1800-869-877
              </div>
            </div>
            <div class="flex mt-6 space-x-4">
              <div>
                <img src="@/assets/images/location.svg" alt="" srcset="" />
              </div>
              <div class="text-[#201F23] mt-10 text-xl font-bold">
                102 Street, India
              </div>
            </div>
            <div class="text-[#201F23] mt-16 text-4xl font-bold">
              Social Media Channel
            </div>
            <div class="flex justify-between w-1/2 mt-10">
              <img src="@/assets/images/Facebook.svg" alt="" srcset="" />
              <img src="@/assets/images/Twitter.svg" alt="" srcset="" />
              <img src="@/assets/images/Github.svg" alt="" srcset="" />
              <img src="@/assets/images/Linkedin.svg" alt="" srcset="" />
            </div>
          </div>
          <div class="m-20">
            <Contact_Form />
          </div>
        </div>
      </div>
    </div>
    <div>
      <div class="w-full flex justify-center">
        <div class="w-4/5 mt-20 flex justify-between mb-20">
          <div class="text-[#201F23] text-xl font-bold">
            2021-2022 © Course Pro Private Limited
          </div>
          <div class="flex space-x-14">
            <div class="text-[#201F23] text-xl font-bold">Term & Condition</div>
            <div class="text-[#201F23] text-xl font-bold">Privacy Policy</div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
import Contact_Form from "./Contact_Form.vue";
export default {
  components: { Contact_Form },
};
</script>
