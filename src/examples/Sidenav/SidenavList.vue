<template>
  <div
    class="w-auto h-auto collapse navbar-collapse max-height-vh-100 h-100"
    id="sidenav-collapse-main"
  >
    <ul class="navbar-nav">
      <li class="mt-3 nav-item text-center ">
        <h6
          class="text-s text-white text-uppercase font-weight-300 "
          :class="this.$store.state.isRTL ? 'me-4' : ''"
        >
          GENERAL
      </h6>
      </li>
      <li class="nav-item">
        <sidenav-collapse navText="" :to="{ name: 'Dashboard' }">
          <template #icon>
            <category />
          </template>
        </sidenav-collapse>
      </li>
      <li class="nav-item">
        <sidenav-collapse navText="" :to="{ name: 'My Invoices' }">
          <template #icon>
            <driver />
          </template>
        </sidenav-collapse>
      </li>
      <li class="nav-item">
        <sidenav-collapse navText="" :to="{ name: 'Tables' }">
          <template #icon>
            <group />
          </template>
        </sidenav-collapse>
      </li>

      <li class="nav-item">
        <sidenav-collapse
          navText=""
          :to="{ name: 'Virtual Reality' }"
        >
          <template #icon>
            <message />
          </template>
        </sidenav-collapse>
      </li>
      <li class="nav-item">
        <sidenav-collapse navText="" :to="{ name: 'Rtl' }">
          <template #icon>
            <percentage />
          </template>
        </sidenav-collapse>
      </li>
      <li class="nav-item">
        <sidenav-collapse navText="" :to="{ name: 'Rtl' }">
          <template #icon>
            <avatar />
          </template>
        </sidenav-collapse>
      </li>
      <li class="mt-3 nav-item text-center">
        <h6
          class="text-s text-white text-uppercase font-weight-300"
          :class="this.$store.state.isRTL ? 'me-4' : ''"
        >
          PRO
        </h6>
      </li>
      <li class="nav-item">
        <sidenav-collapse navText="" :to="{ name: 'Profile' }">
          <template #icon>
            <pro-one />
          </template>
        </sidenav-collapse>
      </li>
      <li class="nav-item">
        <sidenav-collapse navText="" :to="{ name: 'Sign In' }">
          <template #icon>
            <pro-two />
          </template>
        </sidenav-collapse>
      </li>
    </ul>
  </div>
  <!-- <div class="pt-3 mx-3 mt-3 sidenav-footer">
    <sidenav-card
      :class="cardBg"
      textPrimary="Need Help?"
      textSecondary="Please check our docs"
      route="https://www.creative-tim.com/learning-lab/vue/overview/soft-ui-dashboard/"
      label="Documentation"
      icon="ni ni-diamond"
    />
    <a
      class="btn bg-gradient-success mt-4 w-100"
      href="https://www.creative-tim.com/product/vue-soft-ui-dashboard-pro?ref=vsud"
      type="button"
      >Upgrade to pro</a
    >
  </div> -->
</template>
<script>
import SidenavCollapse from "./SidenavCollapse.vue";
// import SidenavCard from "./SidenavCard.vue";
import Category from "../../components/Icon/Category.vue";
import Driver from "../../components/Icon/Driver.vue";
import Group from "../../components/Icon/Group.vue";
import Message from "../../components/Icon/Message.vue";
import ProOne from "../../components/Icon/ProOne.vue";
import ProTwo from "../../components/Icon/ProTwo.vue";
import Avatar from "../../components/Icon/Avatar.vue";
import Percentage from "../../components/Icon/Percentage.vue";

export default {
  name: "SidenavList",
  props: {
    cardBg: String,
  },
  data() {
    return {
      title: "Soft UI Dashboard PRO",
      controls: "dashboardsExamples",
      isActive: "active",
    };
  },
  components: {
    SidenavCollapse,
    Driver,
    Category,
    Group,
    Message,
    ProOne,
    ProTwo,
    Avatar,
    Percentage,
  },
  methods: {
    getRoute() {
      const routeArr = this.$route.path.split("/");
      return routeArr[1];
    },
  },
};
</script>
