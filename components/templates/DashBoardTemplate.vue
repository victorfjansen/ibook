<template>
  <div class="wrapper">
    <div class="ilustration">
      <img src="@/assets/img/dashboard.svg" alt="Dashboard Ilustration" />
      <PageTitle title="Você está no " strong="DashBoard!" />
    </div>

    <button class="button">Logout</button>
  </div>
</template>

<style scoped>
.wrapper {
  position: absolute;
  top: 30%;
  left: 30%;
  display: grid;
  gap: 2.5rem;
  justify-content: center;
}
.ilustration {
  text-align: center;
}

.button {
  background: #292929;
  width: 111px;
  height: 40px;
  margin: 0 auto;
  font-style: 'Montserrat';
  font-size: 22px;
  font-weight: bold;
  color: white;
  cursor: pointer;
  transition: ease 0.3s;
}

.button:hover {
  opacity: 0.9;
}
</style>
