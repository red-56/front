<template>
  <div class="wrapper" :class="{ 'nav-open': $sidebar.showSidebar }">
    <notifications></notifications>

    <side-bar>
      <mobile-menu slot="content"></mobile-menu>
      <sidebar-link to="/d/dashboard">
        <md-icon>dashboard</md-icon>
        <p>Dashboard</p>
      </sidebar-link>
      <sidebar-link to="/d/user">
        <md-icon>person</md-icon>
        <p>User Profile</p>
      </sidebar-link>
      <sidebar-link to="/d/timemanager">
        <md-icon>content_paste</md-icon>
        <p>Time Manager</p>
      </sidebar-link>
      <sidebar-link to="/d/teamgraph">
        <md-icon>library_books</md-icon>
        <p>Team Graph</p>
      </sidebar-link>
      <sidebar-link to="/d/usergraph">
        <md-icon>bubble_chart</md-icon>
        <p>User Graph</p>
      </sidebar-link>
      <sidebar-link to="/d/usermanager">
        <md-icon>supervisor_account</md-icon>
        <p>User Manager</p>
      </sidebar-link>
    </side-bar>

    <div class="main-panel">
      <top-navbar></top-navbar>

      <dashboard-content> </dashboard-content>

      <content-footer v-if="!$route.meta.hideFooter"></content-footer>
    </div>
  </div>
</template>
<style lang="scss"></style>
<script>
import TopNavbar from "./TopNavbar.vue";
import DashboardContent from "./Content.vue";


export default {
  components: {
    TopNavbar,
    DashboardContent
  }
};
</script>
