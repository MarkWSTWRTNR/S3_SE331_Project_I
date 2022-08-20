<template>
  <p>Name: {{ event.name }} {{event.surname}}</p>
  <p>Age: {{ event.age }}</p>
  <p>Home Town: {{ event.homeTown }}</p>
</template>

<script>
export default {
  props: ['event']
}
</script>
