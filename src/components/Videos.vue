<template>
    <div>
        <el-table :data="tableData" style="width: 100%">
            <el-table-column prop="date" label="日期">
            </el-table-column>
            <el-table-column prop="name" label="视频名称">
            </el-table-column>
            <el-table-column prop="url" label="视频地址">
            </el-table-column>
            <el-table-column inline-template :context="_self" label="操作">
                <span>
                    <el-button @click="handleClick(row)" type="text" size="small">查看</el-button>
                    <el-button type="text" size="small">编辑</el-button>
                </span>
            </el-table-column>
        </el-table>
    </div>
</template>
<script>
import https from '../lib/https'

export default {
    data() {
        return {
            tableData:[{
              date: "2016年12月1日",
              name: "阿三开挂集锦",
              url: "http://baidu.com"
            }, {
              date: "2016年12月1日",
              name: "阿三开挂集锦",
              url: "http://baidu.com"
            }]
        }
    },
    methods: {
        handleClick(row) {
            console.log(https.videos);
        }
    },
    mounted() {

    },
    computed: {

    }
}
</script>
