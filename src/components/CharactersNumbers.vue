
<script>
import {store} from '../store' 
export default {
    name: 'CharactersNumbers',
    data() {
        return {
            store,
        }
    },
    computed: {
        returnNumber(){
            return store.characters.length
        }
    },
}
</script>
<template >
    <div class="characters_numbers p-3 mb-3">
        <h3>Found {{returnNumber}} characters</h3>
    </div>
</template>
<style lang="scss" scoped>
     .characters_numbers{
        background-color: #212529;
        h3{
            font-weight: bold;   
        }
        font-weight: bold;
    }
</style>