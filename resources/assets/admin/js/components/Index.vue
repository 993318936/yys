<template>
    <div class="index text-center">
        <div class="login">
        <el-form ref="form" :model="form" label-width="80px">
            <el-form-item label="Account">
                <el-input v-model="form.account" placeholder=""></el-input>
            </el-form-item>
            <el-form-item label="password">
                <el-input v-model="form.name"></el-input>
            </el-form-item>
            <el-form-item>
                <el-button type="primary" @click="onSubmit">登录</el-button>
                <el-button>取消</el-button>
            </el-form-item>
        </el-form>
        <!--<div class="red to-books">-->
            <!--<router-link :to="{name:'listOfBooks'}">Hot searching >></router-link>-->
        <!--</div>-->
        </div>
    </div>
</template>
<script>
    export default {
        data() {
            return {
                form: {
                    account: '',
                    pwd:''

                }
            }
        },
        methods: {
            onSubmit() {
                console.log('submit!');
            }
        }
    }
</script>