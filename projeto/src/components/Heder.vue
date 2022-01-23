<template>
    <div class="Heder">
        <h1>oi</h1>
       <h1>{{ msg }}</h1> 
    </div>
</template>

<script>
export default {
    name: 'Heder',
    props: {
        msg: String
    }
    
}
</script>