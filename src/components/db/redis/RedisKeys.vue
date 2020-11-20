<template>
    <h1>可操作删除</h1>
    <el-table
            :data="tableData"
            style="width: 100%"
            max-height="250">
        <el-table-column
                fixed
                prop="key"
                label="KEY"
                width="150">
        </el-table-column>
        <el-table-column
                prop="type"
                label="TYPE"
                width="120">
        </el-table-column>


        <el-table-column
                fixed="right"
                label="操作"
                width="120">
            <template slot-scope="scope">
                <el-button
                        @click.native.prevent="deleteRow(scope.$index, tableData)"
                        type="text"
                        size="small">
                    移除
                </el-button>
                <el-button
                        @click.native.prevent="deleteRow(scope.$index, tableData)"
                        type="text"
                        size="small">
                    详情
                </el-button>
            </template>
        </el-table-column>
    </el-table>
</template>

<script>
    export default {
        methods: {
            deleteRow(index, rows) {
                rows.splice(index, 1);
            },

            detail(rows) {

            }

        },
        data() {
            return {
                tableData: [{
                    key: 'user:10001',
                    type: 'hash',

                }]
            }
        }
    }
</script>
