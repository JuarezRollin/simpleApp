<template> 
    <!-- the emit function can acces the out variable by throwing a SubmitBtn value then will recieve it outside the components -->
    <button class="button login__submit" @click="$emit('SubmitBtn')">
        <span class="button__text">Log In Now</span>
        <i class="button__icon fas fa-chevron-right"></i>
    </button>		
</template>