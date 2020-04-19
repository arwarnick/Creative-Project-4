<template>
<div class="contact">
  <div class="contact-page">
    <div class="contact-page-item">
      <h2>Address</h2>
      <p>999 Supercar Drive<br>
      Rome, Italy 99999</p>
    </div>
    <div class="contact-page-item">
      <h2>Email</h2>
      <p>greatestsupercars@supercar.com</p>
    </div>
    <div class="contact-page-item">
      <h2>Phone</h2>
      <p>999-999-9999</p>
    </div>
  </div>
</div>
</template>

<style scoped>
.contact-page {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}

.contact-page h2 {
  font-family: "Arial Black", Gadget, sans-serif;
  font-size: 30px;
}

.contact-page p {
  font-size: 20px;
}

.contact-page-item {
  display: flex;
  flex-direction: column;
  align-items: center;
}
</style>
