<template>
  <nav
    class="shadow-none navbar navbar-main navbar-expand-lg border-radius-xl"
    v-bind="$attrs"
    id="navbarBlur"
    data-scroll="true"
  >
    <div class="px-3 py-1 container-fluid">
      <breadcrumbs :currentPage="currentRouteName" :textWhite="textWhite" />
      <div
        class="mt-2 collapse navbar-collapse mt-sm-0 me-md-0 me-sm-4"
        :class="this.$store.state.isRTL ? 'px-0' : 'me-sm-4'"
        id="navbar"
      >
        <div
          class="d-flex align-items-center gap-2 navRightMenuGroup"
          :class="this.$store.state.isRTL ? 'me-md-auto' : 'ms-md-auto'"
        >
          <div>
            <span class="IconBodyDeploy">
            Deploy Now</span>
          </div>
          <div>
            <span class="IconBodyWallet"
              ><img class="walletIcon" src="../../assets/img/icons/vuesax-outline-wallet-add.png" alt="">Balance: $160.56 USD</span>
            <!-- <span
              class="form-control"
            >Balance: $160.56 USD</span> -->
          </div>
          <div>
            <span class="IconBodyShoppingCart"
              ><img class="shoppingCard" src="../../assets/img/icons/cart.png" alt=""></span>
          </div>
        </div>
        <!-- <ul class="navbar-nav justify-content-end">
          <li class="px-3 nav-item d-flex align-items-center">
            <a
              class="p-0 nav-link"
              @click="toggleConfigurator"
              :class="textWhite ? textWhite : 'text-body'"
            >
            <img class="shoppingCard" src="../../assets/img/icons/cart.png" alt="">
            </a>
          </li>
        </ul> -->
      </div>
    </div>
  </nav>
</template>
<script>
import Breadcrumbs from "../Breadcrumbs.vue";
import { mapMutations, mapActions } from "vuex";

export default {
  name: "navbar",
  data() {
    return {
      showMenu: false,
    };
  },
  props: ["minNav", "textWhite"],
  created() {
    this.minNav;
  },
  methods: {
    ...mapMutations(["navbarMinimize", "toggleConfigurator"]),
    ...mapActions(["toggleSidebarColor"]),

    toggleSidebar() {
      this.toggleSidebarColor("bg-white");
      this.navbarMinimize();
    },
  },
  components: {
    Breadcrumbs,
  },
  computed: {
    currentRouteName() {
      return this.$route.name;
    },
  },
  updated() {
    const navbar = document.getElementById("navbarBlur");
    window.addEventListener("scroll", () => {
      if (window.scrollY > 10 && this.$store.state.isNavFixed) {
        navbar.classList.add("blur");
        navbar.classList.add("position-sticky");
        navbar.classList.add("shadow-blur");
      } else {
        navbar.classList.remove("blur");
        navbar.classList.remove("position-sticky");
        navbar.classList.remove("shadow-blur");
      }
    });
  },
};
</script>
