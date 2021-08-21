<template>
    <article @click="router.push('/plant')"  id="card">
        <img src="@/assets/img/basil.png" alt="" >
        <div class="content">
            <h1 class="title">Plant Name</h1>
            <h3 class="type">Plant Type</h3>
            <span class="status thirsty">Thirsty</span>
        </div>
    </article>
</template>

<script>
import { useRouter } from 'vue-router'
export default {
    name: 'card',
    data: ()=> ({

    }),
    setup() {
        const router = useRouter()
        return {
            router
        }
    }
}
</script>

<style scoped lang="scss"> 
    #card {
        width: 95vw;
        height: 160px;
        float: right;
        background: #0B5345;
        border-radius: 40px 0px 0px 40px;
        margin-bottom: 20px;
        display: flex;
        flex-direction: row;
        img {
            position: relative;
            width: 125px;
            height: 125px;
            left: -20px;
            top: 30px;
            overflow: hidden;
        }
        .content {
            width: 100%;
            margin: 20px;
            .title {
                font-style: normal;
                font-weight: bold;
                font-size: 24px;
                color: #FFFFFF;
            }
            .type {
                font-style: normal;
                font-weight: bold;
                font-size: 10px;
                margin-top: 12px;
                color: #C4C4C4;
            }
            .status {
                width: 100px;
                height: 21px;
                box-sizing: border-box;
                border-radius: 50px;
                text-align: center;
                font-style: normal;
                font-weight: 500;
                font-size: 12px;
                &.thirsty {
                    color: #BEA624;
                    border: 1px solid #BEA624;
                    background: rgba(190, 166, 36, 0.5);
                }
                &.healthy {
                    color: #0B5345;
                    border: 1px solid #45B39D;
                    background: rgba(69, 179, 157, 0.5);
                }
            }
        }
    }
</style>