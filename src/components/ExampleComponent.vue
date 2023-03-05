<!-- what problems is vue 3 trying to solve?
1. code that belongs together logically is split up into multiple 
options(data, methods, computed)
2. re-using logic across components can be tricky 

setup method replaces those options(data, methods, computed, watch)

composition 

-->

<template>
    <div>{{ userName }}</div>
    <div>{{ user.name }}</div>
</template>

<script>
    import { ref, reactive } from 'vue';
    export default {

        // data(){
        //     userName: 'nate'
        // }

        setup() {
            //creates a reference, a reactive value
          const userName = ref('default');
          const user = reactive({
            name: 'nate',

          })

          return {userName, user}
        }

    }

</script>