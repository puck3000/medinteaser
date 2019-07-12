<template>
    <div class="logo">
        <div id="dot">●</div>
        <div id="name">
            <h1>MEDIN</h1>
        </div>  
        <div id="zusatz">
            <h2>Biel / Bienne</h2>    
        </div>  
        
    </div>
   
</template>

<script>
export default {

}
</script>

<style lang="stylus" scoped>

h1size = 5

h1, h2
    margin: 0

h1 
    font-size: h1size rem
h2 
    font-size: "calc(%srem / 2)" % h1size 
    font-weight: 50

#dot 
    color: lightblue
    font-size: "calc(%srem)" % h1size  
    margin-left: "calc(%s * 29.8px )" % h1size
    line-height: .5
    transform: scale(1);
    transform-origin: 24.5%;
    transition: transform 2s ease-in-out 
    &:hover
        transform: scale(10) 
    
</style>
