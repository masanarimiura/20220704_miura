<template>
  <div class="container">
    <div class="container__students">
      <h2>生徒一覧</h2>
      <NuxtLink to="/students">生徒情報を見る</NuxtLink>
    </div>
    <div class="container__management">
      <h2>管理者</h2>
      <NuxtLink to="/management">管理画面を見る</NuxtLink>
    </div>
  </div>
</template>

<style>
.container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}
</style>