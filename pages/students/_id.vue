<template>
  <div class="student_id">
    <h2 v-for="student in students" :key="student" v-if="student.id === $route.params.id">{{student.name}}</h2>
    <div><NuxtLink to="/students">生徒一覧へ戻る</NuxtLink>|<NuxtLink to="/">トップページへ</NuxtLink></div>
  </div>
</template>


<script>
export default {
  validate({ params }) {
    return /^[a-z0-9]+$/.test(params.id)
  },
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
  }
};
</script>


<style>
.student_id {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  flex-flow: column;
  justify-content: center;
  align-items: center;
  text-align: center;
}
</style>
