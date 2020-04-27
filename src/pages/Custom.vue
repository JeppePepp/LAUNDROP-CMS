<template>
    <CustomizedLayout>
        <div class="text-3xl font-semibold flex items-center justify-center">
            <Topic :topic='topic'/>
        </div>
        <div class="paragraph text-sm">
            Posted by Laundrop <br> Apil 22, 2020 / Stockholm <br>4 min read
        </div>
        <g-image class="w-8/12 h-2/3 ml-64" src="~/assets/images/cleaning cloth.jpg"></g-image>
        
    </CustomizedLayout>
    
</template>

<script>
import CustomizedLayout from '~/layouts/Customized';
import Topic from "@/components/Topic"

    export default {
        components: {
            CustomizedLayout,
            Topic
        },
        data(){
            return{
                topic:'HUR DU RENGÖRER KLÄDER RÄTT'
            }
        }
        
    }
</script>

<style>
    .paragraph{
        padding-left: 533px; 
    }
</style>