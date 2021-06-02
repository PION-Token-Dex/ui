<template>


  <div class="hasmetamask">
    <div class="popup" id="popup">
      <div class="popup-inner">

        <div class="pion">
          <img src="./assets/img/bgrnd.jpg" alt="" width="100%" class="bgrnd">
        </div>
      </div>

    </div>
  </div>


</template>

<script>

export default {
  name: 'APP',
  created: function () {
    this.interval = setInterval(() => this.refreshData(), 3000);
  },
  data: function () {
    return {
      userAddress: 'Connect to Metamask, then reload.',
    };
  },
  beforeMount() {
    this.refreshData();
  },
  methods: { },
};
</script>

<style>
body {background:none transparent !important;}

</style>
