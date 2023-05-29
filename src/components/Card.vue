<template>
    <div class="card">
        <slot name="title"></slot>
        <header id="header">
            <slot name="header"> </slot>
        </header>
        <body>
            <slot name="body"></slot>
        </body>
        <footer>
            <slot name="footer"></slot>
        </footer>
    </div>
</template>

<script>
export default {
    name:`Card`
}
</script>

<style scoped>
.card{
    border: 2px solid;
width: 406px;
height: 450px;
align-content: center;
margin: 3px;
align-items: center;
/* display: inline-block; */
/* display: flex; */

}

#header img{
    width: 100%;
}
</style>