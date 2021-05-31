<template>
  <div class="wrapper wrapper-content">
    <div class="row">
      <div class="col-lg-2">
        <div class="ibox float-e-margins">
          <div class="ibox-title">
            <span class="label label-success pull-right">Monthly</span>
            <h5>Views</h5>
          </div>
          <div class="ibox-content">
            <h1 class="no-margins">386,200</h1>
            <div class="stat-percent font-bold text-success">98% <i class="fa fa-bolt"></i></div>
            <small>Total views</small>
          </div>
        </div>
      </div>
      <div class="col-lg-2">
        <div class="ibox float-e-margins">
          <div class="ibox-title">
            <span class="label label-info pull-right">Annual</span>
            <h5>Orders</h5>
          </div>
          <div class="ibox-content">
            <h1 class="no-margins">80,800</h1>
            <div class="stat-percent font-bold text-info">20% <i class="fa fa-level-up"></i></div>
            <small>New orders</small>
          </div>
        </div>
      </div>

      <div class="col-lg-4">
        <div class="ibox float-e-margins">
          <div class="ibox-title">
            <span class="label label-primary pull-right">Today</span>
            <h5>visits</h5>
          </div>
          <div class="ibox-content">

            <div class="row">
              <div class="col-md-6">
                <h1 class="no-margins">406,42</h1>
                <div class="font-bold text-navy">44% <i class="fa fa-level-up"></i> <small>Rapid pace</small></div>
              </div>
              <div class="col-md-6">
                <h1 class="no-margins">206,12</h1>
                <div class="font-bold text-navy">22% <i class="fa fa-level-up"></i> <small>Slow pace</small></div>
              </div>
            </div>

          </div>
        </div>
      </div>
    </div>
    <div class="row">
      <div class="col-lg-2">
        <button
          type="button"
          class="btn btn-block btn-primary"
          @click="changeSkinDefault"
        >Change Skin - Default</button>
        <button
          type="button"
          class="btn btn-block btn-primary"
          @click="changeSkin1"
        >Change Skin - 1</button>
        <button
          type="button"
          class="btn btn-block btn-primary"
          @click="changeSkin2"
        >Change Skin - 2</button>
        <button
          type="button"
          class="btn btn-block btn-primary"
          @click="changeSkin3"
        >Change Skin - 3</button>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Home",
  data() {
    return {
      msg: "Welcome to Your Vue.js App",
    };
  },
  methods: {
    changeSkin3() {
      document.querySelector("body").className = "skin-3";
    },
    changeSkin2() {
      document.querySelector("body").className = "light-skin ";
    },
    changeSkin1() {
      document.querySelector("body").className = "skin-1";
    },
    changeSkinDefault() {
      document.querySelector("body").className = "";
    },
  },
};
</script>

