<script setup>

// defineProps(['type','msg']);
//  const type = 'error'
//     const msg = 'This is an alert message'

defineProps({
    type:{
        type:String,
        default:'info',

        
    },
    msg:{
        type:String,
        default:'This is a default message',
    },
});

const getColorClasses =()=>{
    return{
        'info':'bg-blue-100 text-blue-800'
        
    }
}


</script>

<template>
    <div class="p-4 mb-4 text-sm  rounded-lg bg-blue-50 dark:bg-gray-800 dark:text-blue-400" role="alert">
  <span class="font-medium">{{ msg }}</span> 
</div>
 
</template>

<style scoped>

</style>