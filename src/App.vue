<template>
  <section>
    <!-- Interpolation ด้วย Data-->  
    <!-- {{firstname}} -->

    <h1>ชื่อ : {{firstname}}</h1>  
    <h1>นามสกุล : {{lastname}}</h1>
    <h1>อายุ : {{age}} ปี</h1>
    <p>ที่อยู่ : <span v-html="address"></span></p> 
    <!-- ใช้ "v-html" เพื่ออ่านค่าแท็ก HTML-->
  </section>
</template>

<script>


export default {
  name: 'App',
  // ฟังชั่นก์ data จะส่งค่ากลับมาในรูปแบบ Object โดยค่าหรือข้อมูลที่ส่งกลับมานั่นสามารถนำไปใช้ใน template หรือ ส่วนอื่นๆของ Component
  data(){
    return{
      firstname:"พีรพัฒน์",
      lastname:"ตั้งปัญญาไว",
      age:21,
      address:"<strong>กรุงเทพมหานคร</strong>"
    }

  }

}
</script>

<style></style>
