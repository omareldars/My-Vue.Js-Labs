<template>
    <div class="row">
        <table class="table table-striped col-12">
            <thead>
                <tr>
                    <th>ID</th>
                    <th>Name</th>
                    <th>City</th>
                </tr>
            </thead>
            <tbody>
                <tr v-for="student in students" :key="student.id">
                    <td>{{student.id}}</td>
                    <td>{{student.name}}</td>
                    <td>{{student.city}}</td>
                </tr>
            </tbody>
            <tfoot>
                <tr>
                    <td colspan="3">
                        <a @click.prevent="addstudent" href="#" class="btn btn-success text-center w-100">Add New Student</a>
                    </td>
                </tr>

                <tr>
                    <td colspan="3">
                        <h5 class="alert alert-info text-center">{{message}}{{students.length}}</h5>
                    </td>
                </tr>
            </tfoot>
        </table>
    </div>
</template>
<script>
import students from '../students'
import addcomponent from './addcomponent.vue'
export default {
    data(){
        return{
            message:'Total No. of Students = ',
            students:students,

        }
    },
    methods:{
        addstudent(){
            this.students.push({id:this.students[this.students.length-1].id+100,name:'Newly Added',city:'New City'});
        }
    },
    components:{
        addcomponent
    }
}
</script>