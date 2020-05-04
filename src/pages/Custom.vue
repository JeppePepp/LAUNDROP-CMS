<template>
    <CustomizedLayout>
        <div class="text-3xl font-semibold flex items-center justify-center mx-auto container">
            <Topic :topic='topic'/>
        </div>
        <div class="paragraph text-sm">
            Posted by Laundrop <br> Apil 22, 2020 / Stockholm <br>4 min read
        </div>

        <g-image class=" mt-4 w-8/12 h-2/3 ml-64" src="~/assets/images/cleaning cloth.jpg"></g-image>

        <div class="ml-64 mr-64 mt-4 text-justify">
            <TextInput :description = 'description'/>
            <TextInput :description = 'description' class="mt-4"/>
            <TextInput :description = 'description' class="mt-4"/>
        </div>

        <g-image class=" mt-4 w-8/12 h-2/3 ml-64" src="~/assets/images/detergent.jpg"></g-image>

        <div class="ml-64 mr-64 mt-4 text-justify">
            <TextInput :description = 'description'/>
            <TextInput :description = 'description' class="mt-4"/>
            <TextInput :description = 'description' class="mt-4"/>
        </div>     
    </CustomizedLayout>
</template>

<script>
import CustomizedLayout from '~/layouts/Customized';
import Topic from "@/components/Topic";
import TextInput from "@/components/TextInput";

    export default {
        components: {
            CustomizedLayout,
            Topic,
            TextInput
        },
        data(){
            return{
                topic:'HUR DU RENGÖRER KLÄDER RÄTT',
                description: 'Culpa Lorem ea do elit enim reprehenderit duis dolore. Lorem exercitation consequat consequat' + 
                'incididunt nisi consectetur nulla ea id. Consectetur minim esse veniam velit id commodo amet dolor'+
                'voluptate non et do. Do ipsum eiusmod ex anim nulla duis. Duis eiusmod labore labore labore elit'+
                'do labore culpa culpa aliquip mollit est duis adipisicing.'+
                'Culpa Lorem ea do elit enim reprehenderit duis dolore. Lorem exercitation consequat consequat' + 
                'incididunt nisi consectetur nulla ea id. Consectetur minim esse veniam velit id commodo amet dolor'+
                'voluptate non et do. Do ipsum eiusmod ex anim nulla duis. Duis eiusmod labore labore labore elit'+
                'do labore culpa culpa aliquip mollit est duis adipisicing.'
            }
        }
        
    }
</script>

<style>
    .paragraph{
        padding-left: 533px; 
    }
    .marginTop{
        margin-top: 10px;
    }
</style>