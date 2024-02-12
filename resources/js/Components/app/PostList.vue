<script setup>
import PostItem from "@/Components/app/PostItem.vue";

const post1={
    user:{
        id:1,
        avatar:'https://i.pravatar.cc/100',
        name:'Shivansh Goswami'
    },
    group:null,
    attachments:[
        {
            id:1,
            name:'test.png',
            url:'https://i.pravatar.cc/1000',
            mime:'image/png',
        },
        {
            id:2,
            name:'test2.png',
            url:'https://i.pravatar.cc/1000',
            mime:'image/png',
        },
        {
            id:3,
            name:'Mydoc.doc',
            url:'#',
            mime:'application/msword',
        }
    ],
    body:`<p>
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Enim exercitationem pariatur, porro odit ratione recusandae numquam. Maxime, praesentium asperiores, corporis ipsam adipisci cupiditate commodi nesciunt, ex maiores vitae possimus quaerat?
        </p>
        
        <p>
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Enim exercitationem pariatur, porro odit ratione recusandae numquam. Maxime, praesentium asperiores, corporis ipsam adipisci cupiditate commodi nesciunt, ex maiores vitae possimus quaerat?
        </p>`,
    created_at:'2023-02-02 15:12',
    
}
const post2={
    user:{
        id:1,
        avatar:'https://i.pravatar.cc/100',
        name:'Amrut Goswami'
    },
    group:{
        id:1,
        name:'Laravel Developers'
    },
    body:`<p>
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Enim exercitationem pariatur, porro odit ratione recusandae numquam. Maxime, praesentium asperiores, corporis ipsam adipisci cupiditate commodi nesciunt, ex maiores vitae possimus quaerat?
        </p>
        
        <p>
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Enim exercitationem pariatur, porro odit ratione recusandae numquam. Maxime, praesentium asperiores, corporis ipsam adipisci cupiditate commodi nesciunt, ex maiores vitae possimus quaerat?
        </p>`,
    created_at:'2023-02-02 15:12',
    
}
 
</script>
<template>
<div>
    <div class="overflow-auto">
        <PostItem :post="post1"/>
        <PostItem :post="post2"/>
        <PostItem :post="post1"/>
        <PostItem :post="post1"/>
    </div>
</div>

</template>

<style>

</style>