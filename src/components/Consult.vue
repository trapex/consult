<script setup>

</script>

<template>
    <div class="consult">
      <div class="consult-first-screen container">
        <div class="consult-content">
            <div class="consult-title">Empowering your business through 
                <br>
                expert 
                <span>IT-Consulting</span>
            </div>
          <div class="consult-text">Delivering comprehensive, tailored, and strategic IT-solutions to help your business navigate, adapt, and overcome the complex challenges of today's digital landscape</div>
        </div>
        <div class="consult-img">
          <img alt="a-consult happy man" src="@/assets/img/happy-man.png" />
        </div>
      </div>
      <div class="container">
        <div class="consult-trust">
        <div class="consult-trust-title">Trusted by</div>
        <div class="consult-trust-list">
          <div><img alt="acme logo" src="@/assets/img/acme-logo.png" /></div>
          <div><img alt="aven logo" src="@/assets/img/aven-logo.png" /></div>
          <div><img alt="asgardia logo" src="@/assets/img/asgardia-logo.png" /></div>
          <div><img alt="atica logo" src="@/assets/img/atica-logo.png" /></div>
          <div><img alt="amara logo" src="@/assets/img/amara-logo.png" /></div>
        </div>
      </div>
      </div> 
    </div>
</template>

<style scoped>
.consult {
    margin-top: 20px;
    padding-bottom: 75px;
    background-image: url('/src/assets/img/first-screen-bg.png');
}
.consult-first-screen {
    display: flex;
    justify-content: space-between;
}
.consult-content {
    margin-top: 110px;
    margin-left: 125px;
}
.consult-title {
    font-size: 52px;
    line-height: 1.2;
}
.consult-title span {
    font-weight: 700;
}
.consult-text {
    width: 520px;
    margin-top: 26px;
    font-size: 20px;
    line-height: 2;
}
.consult-trust {
    margin-top: 14px;
    margin-left: 110px;
}
.consult-trust-title {
    font-size: 24px;
    font-weight: 600;
    text-align: center;
    color: var(--black);
}
.consult-trust-list {
    display: flex;
    justify-content: space-around;
    margin-top: 24px;
}
</style>