<template>

    <div :class="book.available ? 'green': 'red' ">
        <h2>Actor Name : {{book.name}}</h2>
        <h4> Age : {{book.age}}</h4>
        <h4>Total Awards Won: {{book.noofawards}}</h4>
        <h4> BirthPlace : {{book.birthplace}}</h4>
        <h4> Living Place : {{book.livingplace}}</h4>
        <img :src= "book.photo" height="300" width="300"/>
        
        
    </div>

</template>

<script>


export default{
    name: 'BookItem',
    props:{
        book: Array
    }
}


</script>

<style scoped>


h4{
    margin: 2px;
}

div{
    background-color: #ffb89e;
    color: black;
    padding: 1em;
    text-align: center;
}

.red{
    background-color: rgb(173, 182, 173) !important;

}
.green{
    color: rgb(12, 12, 12);
    background-color: rgb(173, 182, 173);
}


</style>