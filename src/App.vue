<template>
  <div class="page-wrapper">
    <div class="page">
      <div class="message-history">{{ messageHistory }}</div>
      <div class="message-block">
        <input
          type="text"
          class="message-block__message input"
          v-model="message"
        />
        <img
          src="@/icons/send-message-icon.png"
          alt=""
          class="message-block__send-message-button"
          @click="sendMessage"
        />
      </div>
      <button class="">+</button>
    </div>
  </div>
</template>

<script>
export default {
  name: "App",
  data() {
    return {
      messageHistory:
        "Lorem ipsum dolor sit amet consectetur adipisicing elit. Esse unde blanditiis, atque laboriosam minima distinctio omnis neque architecto exercitationem nisi repudiandae nulla vitae dolore quasi facere modi libero pariatur velit!",
      message: "",
    };
  },
  methods: {
    sendMessage() {
      if (this.message !== "") {
        console.log(this.message);
      }
      this.message = "";
    },
  },
};
</script>

<style>
.page {
  display: flex;
  flex-direction: column;
  padding: 15px;
}
.message-block {
  display: flex;
}
.message-block__send-message-button {
  width: 35px;
}
.input {
  border: 1px solid black;
  width: 40%;
}
</style>
