<template lang="">
    <div id="container">
        <h1>
            <slot>
                
            </slot>
        </h1>




        <!-- <h1>
            <slot>
        
            </slot>
        </h1> -->
    </div>
</template>
<script>
export default {
    
}
</script>
<style>
#container{
    display: flex;
    flex-direction: row;
}
    h1{
        color: blue;
        border: red 2px solid;
        width: 600px;
        margin: 0 auto;
        margin-top: 1em;
    }
</style>