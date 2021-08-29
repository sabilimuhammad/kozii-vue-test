<template>
  <div class="nav-container">
    <nav class="nav container">
      <div class="flex items-center w-full">
        <div class="logo-container">
          <h1>KOZII</h1>
        </div>
        <input
          v-model="searchValue"
          type="text"
          class="kozi-input__control mx-2 w-80"
          placeholder="Search"
        />
      </div>
      <div class="flex items-center">
        <a href="">
          <p class="mx-2">Cart</p>
        </a>
        <a href="">
          <p class="mx-2">Chat</p>
        </a>
        <a href="">
          <p class="mx-2">Notification</p>
        </a>
        <a href="">
          <p class="mx-2">Vouchers</p>
        </a>
        <div class="divider"></div>
        <button class="btn btn-outline mx-2">Login</button>
        <button class="btn mx-2">Register</button>
      </div>
    </nav>
  </div>
</template>

<script>
export default {
  data() {
    return {
      searchValue: "",
    };
  },
};
</script>
