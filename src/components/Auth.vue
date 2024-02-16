<template>
  <div class="page-wrapper">
    <div class="page">
      <input type="email" name="" id="" class="page__email-input input" />
      <input type="password" class="page__password-input input" />
    </div>
  </div>
</template>

<script>
export default {
  name: "App",
};
</script>

<style>
.page-wrapper {
}
.page {
  display: flex;
  flex-direction: column;
  max-width: 1200px;
  align-items: center;
}
.page__email-input {
  margin-bottom: 5px;
}
.page__password-input {
}
.input {
  border: 1px solid black;
  width: 40%;
}