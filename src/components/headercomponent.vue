<template>
    <div class="row">
        <div class="jumbotron col-12">
            <h3>Header Component</h3>
            <p :class="['lead',branch=='Mansoura'?'mansoura':'', branch=='Alex'?'alex':'', branch=='Smart'?'smart':'']">{{iti}} {{branch}} {{branchname}}</p>
        </div>
    </div>
</template>

<script>
// import { defineComponent } from '@vue/composition-api'

export default {
    data(){
        return{
            iti:"ITI",
            branchname:"BRANCH",
        }
       
    },
    props:["branch"]
    ,
    
}
</script>
<style scoped>
.mansoura{
    color:red;
}
.alex{
    color:blue;
}
.smart{
    color:brown;
}
</style>
