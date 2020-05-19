<template>
    <div class="container mt-5">
        <div class="row justify-content-center">
            <div class="col-8">
                <div class="list-group" v-for="(item, index) in articulos" :key="index">
                    
                        <nuxt-link :to="`/Articulos/${item.id}`">{{item.titulo}}</nuxt-link>
                    
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    data(){
        return{
            articulos: [
                {id: 1, titulo: 'Articulo #1'},
                {id: 2, titulo: 'Articulo #2'},
                {id: 3, titulo: 'Articulo #3'},
                {id: 4, titulo: 'Articulo #4'},
                {id: 5, titulo: 'Articulo #5'},
            ]
        }
    },
}
</script>