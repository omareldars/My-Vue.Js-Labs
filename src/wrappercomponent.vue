<template>
    <div class="container mt-2">
        
        <div class="row">
            <div class="col-12">
                <headercomponent branch="Mansoura"/>
            </div> <!-- Mansoura , Alex , Smart-->
        </div> <!-- End of Header-->


        <div class="row">
            <div class="col-4">
                <linkscomponent/>
            </div><!--End of links-->

            <div class="col-8">
               <bodycomponent/>
            </div><!--End of body-->

        </div> <!-- End of Content-->

        <div class="row">
            <div class="col-12">
                <footercomponent/>
            </div>
        </div> <!-- End of Footer-->

    </div><!--End of Conatainer-->
</template>
<script>
import headercomponent from './components/headercomponent.vue'
import linkscomponent from './components/linkscomponent.vue'
import bodycomponent from './components/bodycomponent.vue'
import footercomponent from './components/footercomponent.vue'

export default{
    components:{
        headercomponent,
        linkscomponent,
        bodycomponent,
        footercomponent
    }
}
</script>
