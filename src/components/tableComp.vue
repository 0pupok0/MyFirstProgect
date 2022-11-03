<template>
<div class="table">
    <button-component @click="$root.$emit('p2')" class="btns2">Button</button-component>
    <button-component @click="scrollTo('p2')" class="btns2">Button</button-component>
    <button-component @click="scrollTo('p2')" class="btns2">Button</button-component>
    <button-component @click="scrollTo('p2')" class="btns2">Button</button-component>
    <button-component @click="scrollTo('p2')" class="btns2">Button</button-component>
    <button-component @click="scrollTo('p2')" class="btns2" style="border:none">Button</button-component>
</div>
</template>
<script>
export default{
    name:"tableComp"
    
}
</script>
<style>
.table{
    border: 3px solid black;
    border-radius: 25px;
    background-color: white;
    width: 20vw;
    padding-top: 20px;
    padding-bottom: 20px;
    margin: 20px;
    height:fit-content;
    position: sticky;
    top: 100px;

}
.btns2 {
    background: none;
    border:none;
    text-decoration: none;
    color: #000000;
    width: 100%;
    border-bottom: #cccccc 2px solid;
}
.btns2:hover {
    background-color:  #911e1e;
    text-shadow: 0 0 1px  #911e1e;
}
</style>