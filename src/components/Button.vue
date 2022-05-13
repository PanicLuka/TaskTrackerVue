<template>
    <button @click="$emit('add-task')" :style="{background: color}" class="btn" >
        {{title}}
    </button>
</template>

<script>
export default {
    name: 'Button',
    props: {
        title: String,
        color: String
    },
    // methods: {
    //     onClick(){
    //         // console.log();
    //     }
    // }

}
</script>

