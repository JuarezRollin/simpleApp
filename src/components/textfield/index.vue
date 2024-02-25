<script>
export default{
    // the props components is where you can acces the value/variable that is inside this components and share it outside its scope
    props: {
        //format variable/props : datatype but you can use some default value when using a prop like a variable using an object then set a type and what is its default value
        // text_prop:{
        //     type: 'String or Function or Array etc its all up to you separated by kama',
        //     default: 'its default value'
        // }
        text: String,
        modelValue: String,
        placeholder: String,
  },
}
</script>


<template>
    <div class="login__field">
        <i class="login__icon fas fa-user"></i>
        <input type="text" class="login__input" :placeholder="placeholder" :value="modelValue" @input="(event) => $emit('update:modelValue', event.target.value)">
    </div>
</template>