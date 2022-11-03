<template>
    <div class="box">
        <button-component @click="scrollTo('p2')">efe</button-component>
        <div ref="p1">
        Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aenean sollicitudin pharetra dui, eget rhoncus ligula posuere a. Sed efficitur egestas aliquam. Integer ornare ipsum id orci ultricies, non imperdiet felis eleifend. Aenean vestibulum eros libero, ut feugiat ipsum blandit id. Integer finibus augue vel sapien ultricies elementum. Integer eleifend purus eget tempus varius. Aliquam ornare egestas mollis. Etiam efficitur viverra quam, eu mollis lacus luctus vitae. Morbi eget nisi ut diam maximus finibus vel eget enim. Praesent mollis magna ligula, eu sollicitudin nisl pellentesque vel. Proin dui massa, semper eu rutrum in, varius eu dui. Vivamus nec neque in leo fringilla accumsan in non augue. Duis pretium enim ac scelerisque convallis. In id blandit turpis, vel lobortis arcu. Aliquam dignissim facilisis lorem, id sodales felis convallis ut. Vestibulum a elementum augue.
        Mauris pellentesque turpis tortor, vitae tristique elit fringilla pellentesque. Duis aliquam nunc eu commodo mollis. Curabitur vitae mauris dictum, tempor orci id, ultrices dolor. Aliquam vel arcu purus. Sed ornare risus nec odio mollis, vitae tristique turpis dictum. Integer sollicitudin malesuada mauris, sit amet fermentum arcu viverra quis. Donec ullamcorper erat molestie nunc auctor tempus. Mauris scelerisque erat velit, vitae dignissim mi tincidunt ac. Vestibulum dignissim laoreet malesuada. Proin nec lectus mollis, tincidunt ante eget, eleifend ante. Donec nec neque non risus aliquet efficitur at vel arcu. Mauris vitae justo massa. Vestibulum ante ipsum primis in faucibus orci luctus et ultrices posuere cubilia curae; Suspendisse potenti. Nullam massa diam, vehicula ac tincidunt quis, ullamcorper egestas odio.<br/><br/>
        </div>
        <div ref="p2">
        Nulla sollicitudin accumsan massa, et feugiat diam aliquam eget. Duis eget tellus faucibus, dapibus erat vel, molestie nulla. Suspendisse potenti. Nam molestie tincidunt risus sed interdum. Vestibulum ornare lectus sapien, nec pretium ligula sollicitudin pharetra. Proin et metus nec ex dictum lacinia. Proin a efficitur nulla. Suspendisse potenti. Fusce mollis placerat eros, ut mollis risus euismod quis. Praesent egestas ullamcorper semper. Mauris aliquet viverra nisi, nec rhoncus nisl imperdiet a. Praesent suscipit, magna eget efficitur auctor, quam mi egestas turpis, ac accumsan ligula dolor pellentesque leo. In sed massa vel odio volutpat commodo. Integer commodo turpis nunc, et commodo elit consequat at. Aenean ut felis ornare, fermentum nisl non, tristique urna.Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aenean sollicitudin pharetra dui, eget rhoncus ligula posuere a. Sed efficitur egestas aliquam. Integer ornare ipsum id orci ultricies, non imperdiet felis eleifend. Aenean vestibulum eros libero, ut feugiat ipsum blandit id. Integer finibus augue vel sapien ultricies elementum. Integer eleifend purus eget tempus varius. Aliquam ornare egestas mollis. Etiam efficitur viverra quam, eu mollis lacus luctus vitae. Morbi eget nisi ut diam maximus finibus vel eget enim. Praesent mollis magna ligula, eu sollicitudin nisl pellentesque vel. Proin dui massa, semper eu rutrum in, varius eu dui. Vivamus nec neque in leo fringilla accumsan in non augue. Duis pretium enim ac scelerisque convallis. In id blandit turpis, vel lobortis arcu. Aliquam dignissim facilisis lorem, id sodales felis convallis ut. Vestibulum a elementum augue. Mauris pellentesque turpis tortor, vitae tristique elit fringilla pellentesque. Duis aliquam nunc eu commodo mollis. Curabitur vitae mauris dictum, tempor orci id, ultrices dolor. Aliquam vel arcu purus. Sed ornare risus nec odio mollis, vitae tristique turpis dictum. Integer sollicitudin malesuada mauris, sit amet fermentum arcu viverra quis. Donec ullamcorper erat molestie nunc auctor tempus. Mauris scelerisque erat velit, vitae dignissim mi tincidunt ac. Vestibulum dignissim laoreet malesuada. Proin nec lectus mollis, tincidunt ante eget, eleifend ante. Donec nec neque non risus aliquet efficitur at vel arcu. Mauris vitae justo massa. 
        </div>
        <div ref="p3">vehicula ac tincidunt quis, ullamcorper egestas odio. Nulla sollicitudin accumsan massa, et feugiat diam aliquam eget. Duis eget tellus faucibus, dapibus erat vel, molestie nulla. Suspendisse potenti. Nam molestie tincidunt risus sed interdum. Vestibulum ornare lectus sapien, nec pretium ligula sollicitudin pharetra. Proin et metus nec ex dictum lacinia. Proin a efficitur nulla. Suspendisse potenti. Fusce mollis placerat eros, ut mollis risus euismod quis. Praesent egestas ullamcorper semper. Mauris aliquet viverra nisi, nec rhoncus nisl imperdiet a. Praesent suscipit, magna eget efficitur auctor, quam mi egestas turpis, ac accumsan ligula dolor pellentesque leo. In sed massa vel odio volutpat commodo. Integer commodo turpis nunc, et commodo elit consequat at. Aenean ut felis ornare, fermentum nisl non, tristique urna.
        Vty.urdujr
        </div>
    </div>
</template>

<script>

export default{
    name:"textComp",
    methods: {
        scrollTo(refName) {
            var element = this.$refs[refName];
            var top = element.offsetTop;
            window.scrollTo(0, top - 100);
        }
    },
    mounted() {
        this.$root.$on('p2', this.scrollTo('p2'))
    }
}
</script>

<style>
.box
{
border: 3px solid black;
border-radius: 25px;
padding: 20px;
background-color: white;
width: fit-content;
margin-left: 10vw;
margin-top: 100px;
margin-right: 3vw;
}

</style>