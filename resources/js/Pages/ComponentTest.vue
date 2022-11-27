<script setup>
import GuestLayout from '@/Layouts/GuestLayout.vue';
import InputLabel from '@/Components/InputLabel.vue';
import TextInputVue from '@/Components/TextInput.vue';

const emitTest = e => console.log(e);
</script>

<template>
  <GuestLayout>
    <InputLabel value="件名">タイトル</InputLabel>
    <TextInputVue modelValue="初期値が入ります" 
      @update:modelValue="emitTest"
    ></TextInputVue><br>
    何か文字を書く
  </GuestLayout>
</template>