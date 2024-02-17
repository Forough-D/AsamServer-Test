<template>
  <nav aria-label="breadcrumb">
    <h6 class="mb-0 font-weight-bolder" :class="textWhite ? 'text-white' : ''">
      {{ currentPage }}
    </h6>
    <ol
      class="px-0 pt-1 pb-0 mb-0 bg-transparent breadcrumb"
      :class="this.$store.state.isRTL ? '' : ' me-sm-6'"
    >
      <li class="text-sm breadcrumb-item" :class="textWhite">
        <img src="../assets/img/icons/vuesax-outline-tag-right.png" alt="">
      </li>
      <li class="text-sm breadcrumb-item" :class="textWhite">
        <a
          v-if="this.$store.state.isRTL"
          :class="textWhite"
          class="opacity-5 ps-2"
          href="dashboard"
          >لوحات القيادة</a
        >
        <a v-else :class="textWhite" class="opacity-8" href="dashboard">Dashboard</a>
      </li>
      <li
        class="text-sm breadcrumb-item active"
        :class="textWhite ? 'text-white' : 'text-dark'"
        aria-current="page"
      >
        {{ currentPage }}
      </li>
    </ol>
    
  </nav>
</template>

<script>
export default {
  name: "breadcrumbs",
  props: {
    currentPage: {
      required: true,
    },
    textWhite: {
      type: String,
    },
  },
};
</script>
