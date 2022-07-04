<template>
  <div class="students">
    <h2>生徒一覧</h2>
    <ul>
      <!-- <li v-for="student in students" :key="student">
        <NuxtLink to="/students/(student.idを代入したいが方法が浮かばない)">{{student.name}}</NuxtLink>
      </li> -->
      <li>
        <NuxtLink to="/students/qnfungqxllc3m1ak">生徒A</NuxtLink>
      </li>
      <li>
        <NuxtLink to="/students/7j9cumkgsq6l264c">生徒B</NuxtLink>
      </li>
      <li>
        <NuxtLink to="/students/eo34bhey9m0d92ou">生徒C</NuxtLink>
      </li>
    </ul>
    <NuxtLink to="/">戻る</NuxtLink>
  </div>
</template>


<script>
export default {
  data() {
    return {
      students: [
        {
          id: "qnfungqxllc3m1ak",
          name: "生徒A",
        },
        {
          id: "7j9cumkgsq6l264c",
          name: "生徒B",
        },
        {
          id: "eo34bhey9m0d92ou",
          name: "生徒C",
        },
      ],
    };
  },
};
</script>


<style>
.students {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  flex-flow: column;
  justify-content: center;
  align-items: center;
  text-align: center;
}
</style>