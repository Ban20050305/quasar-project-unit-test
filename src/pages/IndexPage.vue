<template>
  <div class="htmlClass">
    <h1>{{ title }}</h1>
    <form>
      <input type="text" id="firstName" v-model="firstName" />
      <input type="text" id="lastName" v-model="lastName" />
      <button @click="submitForm()" class="submitForm">Submit</button>
  </form>
  </div>
</template>

<script>
export default {
  name: 'InputPage',
  data() {
    return {
      title: 'วิวัฒนาการของโลกสมัยใหม่.',
      firstName: 'บัณฑิตา',
      lastName: 'สุริยะ',
      nickName:'อีฟ',
      stuCode:'345',
    }
  },
  methods: {
    submitForm() {
      this.$emit('submit form')
    },
  }
}
</script>

<style scoped></style>
