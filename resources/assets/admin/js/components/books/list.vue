<template>
    <div>
        list of books
    </div>
</template>
<script>
    import axios from 'axios'
    export default {
        created(){
            axios.get('./../../../../../../controls/connect.php')
                    .then(function (response) {
                        console.log(response);
                    })
                    .catch(function (error) {
                        console.log(error);
                    });
        }
    }
</script>