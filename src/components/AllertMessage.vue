<template>
  <div class="message" v-bind:class="{'active': isMessageShow}">
      <p>{{ message }}</p>
  </div>
</template>

<script>
export default {
  name: 'MessageInfo',
  props: ['message'],
  data: function () {
    return {
      isMessageShow: false,
    }
  },
  methods: {
    closeMessage () {
      this.isMessageShow = false;
    },
    sendMessage () {
      this.isMessageShow = true;
      setTimeout(this.closeMessage, 3000);
    }
  }
}
</script>