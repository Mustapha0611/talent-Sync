<template>
  <div class="lg:px-[8rem] px-5 py-20 flex flex-col lg:flex-row">
    <section class="flex-1" data-aos="fade-down">
      <h2 class="text-blue-700 text-base font-semibold">Support</h2>
      <h3 class="text-gray-800 text-5xl font-semibold my-3">FAQS</h3>
      <p class="text-gray-500 text-xl">
        Everything you need to know about the product and billing. Can’t find
        the answer you’re looking for? Please
        <span class="decoration-gray-400 underline"
          >chat to our friendly team.</span
        >
      </p>
    </section>
    <section class="flex-1 py-5 lg:px-10 px-2">
      <Accordion :activeIndex="0" expandIcon="pi pi-plus" collapseIcon="pi pi-minus">
        <AccordionTab v-for="tab in tabs">
          <template #header >
            <span class="flex w-full border-b-2 font-semibold text-base p-5 ">
             {{ tab.title }}
            </span>
            
          </template>
          <p class="px-5 text-gray-600 py-2 text-sm">
            {{ tab.content }}
            </p>
        </AccordionTab>
      </Accordion>
    </section>
  </div>
</template>
<script setup>
import { ref } from "vue";
import 'primeicons/primeicons.css'
import Accordion from "primevue/accordion";
import AccordionTab from "primevue/accordiontab";

const tabs = ref([
  {
    title: "How many participants can join a ClearLink video conference?",
    content:
      "ClearLink offers flexible meeting options. Depending on your subscription plan, you can host meetings with varying numbers of participants. Our plans are designed to accommodate small team collaborations and large-scale webinars, ensuring you have the right fit for your needs.",
  },
  {
    title: "Can I use ClearLink on multiple devices?",
    content:
      "ClearLink offers flexible meeting options. Depending on your subscription plan, you can host meetings with varying numbers of participants. Our plans are designed to accommodate small team collaborations and large-scale webinars, ensuring you have the right fit for your needs.",
  },
  {
    title: "Is ClearLink compatible with other video conferencing platforms?",
    content:
      "ClearLink offers flexible meeting options. Depending on your subscription plan, you can host meetings with varying numbers of participants. Our plans are designed to accommodate small team collaborations and large-scale webinars, ensuring you have the right fit for your needs.",
  },
  {
    title: "How does ClearLink ensure the security of my video conferences?",
    content:
      "ClearLink offers flexible meeting options. Depending on your subscription plan, you can host meetings with varying numbers of participants. Our plans are designed to accommodate small team collaborations and large-scale webinars, ensuring you have the right fit for your needs.",
  },
  {
    title: "Do I need to download any software to use ClearLink?",
    content:
      "ClearLink offers flexible meeting options. Depending on your subscription plan, you can host meetings with varying numbers of participants. Our plans are designed to accommodate small team collaborations and large-scale webinars, ensuring you have the right fit for your needs.",
  },
  {
    title:'What kind of customer support does ClearLink provide?', 
    content:
        "ClearLink offers flexible meeting options. Depending on your subscription plan, you can host meetings with varying numbers of participants. Our plans are designed to accommodate small team collaborations and large-scale webinars, ensuring you have the right fit for your needs."
  }
]);
</script>
