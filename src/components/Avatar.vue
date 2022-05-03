<template>
 <div class="avatar-container">
     <img class="avatar-img" :src="imagen" alt="">
     <p class="avatar-name">{{nombre}}</p>
 </div>
</template>

<script>
export default {
    props:['nombre', 'imagen']
}
</script>

<style>
    .avatar-container{
        display: flex;
        align-items: center;
        margin: 1rem;
        gap: 1rem;
    }

    .avatar-img{
        border-radius: 50%;
        max-width: 100px;
    }
    .avatar-name{
        font-size: 2rem;
        color: green;
    }
</style>