<template>
    <div>
        <button class="btn btn-primary" @click.prevent="addstudent">Add</button>
    </div>
</template>
<script>
export default{
    data(){
        return{
            students:[
                {name:"Bermawey",city:"Mit Ghamr"},
                {name:"Ali",city:"Temy Alamdid"},
                {name:"Taha",city:"PortSaed"},
                {name:"Baioumy",city:"Mit Ghamr"}
            ]
        }
    },

}
</script>