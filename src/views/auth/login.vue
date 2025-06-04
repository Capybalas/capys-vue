<template>

    <n-space vertical justify="center" class="space">
        <n-card class="box">
            <n-form :model="account">
                <n-form-item label="邮箱/手机号">
                    <n-input v-model:value="account.account" />
                </n-form-item>

                <n-form-item label="密码">
                    <n-input v-model:value="account.password" type="password" />
                </n-form-item>

                <n-button type="primary" ghost block>登录</n-button>
            </n-form>
        </n-card>
    </n-space>

</template>

<script setup lang="ts">
import type { IAccount } from '@/model/account';
import { ref } from 'vue';


const account = ref<IAccount>({
    account: "",
    password: "",
})

</script>

<style scoped>
.box {
    inline-size: 100%;
    margin-inline: auto;
    max-inline-size: 500px;
}

.space {
    height: calc(100vh - 128px);
}
</style>