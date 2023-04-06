<template>
  <div class="card">
    <div class="avatar">CG</div>
    <p>Name: {{ name }}</p>
    <p>Title: {{ title }}</p>
    <p>Age: {{ age }}</p>
  </div>
</template>
<script>
export default {
  props: {
    name: String,
    title: String,
    age: Number,
  },
};
</script>
<style>
.card {
  width: 15rem;
  height: 16rem;
  border: 1px solid #e5e3e3;
  box-shadow: 10px 10px 10px #efefef;
  padding: 1.5rem;
  border-radius: 0.5rem;
  margin-bottom: 2rem;
  text-align: left;
}
p {
  font-weight: 600;
}
.avatar {
  width: 4rem;
  height: 4rem;
  border: 3px solid lightgray;
  display: flex;
  flex-direction: row;
  justify-content: center;
  align-items: center;
  border-radius: 50%;
  margin: auto;
}
</style>
