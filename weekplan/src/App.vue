<script setup>
import Subject from './components/Subject.vue'
import Break from './components/Break.vue'
</script>

<template class="template">
  <h1 class="title">Plan</h1>
  <table class="plan">
    <td class="day">
      <tr class="title">Monday</tr>
      <tr><Subject subject="Forum" start="0815" end="0945" type="full"/></tr>
      <tr><Subject subject="IM" start="0955" end="1125" type="full"/></tr>
      <tr><Break start="1125" end="1210" type="full"/></tr>
      <tr><Subject subject="English" start="1210" end="1435" type="double"/></tr>
      <tr><Subject subject="IM" start="1445" end="1605" type="full"/></tr>
    </td>
    <td class="day">
      <tr class="title">Tuesday</tr>
      <tr><Subject subject="IG" start="0815" end="1125" type="quad"/></tr>
      <tr><Break start="1125" end="1210"/></tr>
      <tr><Subject subject="Maths" start="1210" end="1255" type="half" /></tr>
      <tr><Subject subject="IM" start="1305" end="1435" type=full /></tr>
    </td>
    <td class="day">
      <tr class="title">Wednesday</tr>
      <tr><Subject subject="None" start="0815" end="0945" type="full"/></tr>
      <tr><Subject subject="Maths" start="0955" end="1125" type="full"/></tr>
      <tr><Break start="1125" end="1210" /></tr>
      <tr><Subject subject="English" start="1210" end="1340" type="full"/></tr>
      <tr><Subject subject="IM" start="1350" end="1520" type="full"/></tr>
    </td>
    <td class="day">
      <tr class="title">Thursday</tr>
      <tr><Subject subject="YFF" start="0815" end="0945" type="full"/></tr>
      <tr><Subject subject="YFF" start="0955" end="1125" type="full"/></tr>
      <tr><Break start="1125" end="1210" /></tr>
      <tr><Subject subject="Midttime" start="1210" end="1255" type="half"/></tr>
      <tr><Subject subject="YFF" start="1205" end="1435" type="full"/></tr>
    </td>
    <td class="day">
      <tr class="title">Friday</tr>
      <tr><Subject subject="IM" start="0815" end="1125" type="quad"/></tr>
      <tr><Break start="1125" end="1210" /></tr>
      <tr><Subject subject="Science" start="1210" end="1340" type="full"/></tr>
      <tr><Subject subject="PE" start="1350" end="1520" type="full"/></tr>
    </td>
  </table>
</template>

<style scoped>
/* center title */
.title {
  text-align: center;
  color: white;
  font-size: x-large;
}

/* center table */
.plan {
  width: 100%;
  height: 100%;
  margin-left: auto;
  margin-right: auto;
  text-align: center;
}

</style>
