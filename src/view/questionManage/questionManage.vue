<template>
  <div>
    <div class="head">
      搜索用户：<Input placeholder="请输入用户名" style="width: auto" />
      <Button style="margin-left:8px;" type="primary">查询</Button>
    </div>
    <Table size="default" border :columns="columns" :data="list"></Table>
  </div>
</template>
<script>
export default {
  name: 'userManage',
  data () {
    return {
      columns: [
        {
          title: '编号',
          key: 'userId',
          width: 100,
          align: 'center'
        },
        {
          title: '用户名',
          key: 'userName',
          align: 'center',
          width: 150
        },
        {
          title: '姓名',
          key: 'name',
          align: 'center',
          width: 120
        },
        {
          title: '性别',
          key: 'gender',
          align: 'center',
          width: 100
        },
        {
          title: '联系电话',
          key: 'telephone',
          align: 'center',
          width: 200
        },
        {
          title: '邮箱地址',
          key: 'email',
          align: 'center',
          width: 200
        },
        {
          title: '备注',
          key: 'remark',
          align: 'center'
        },
        {
          title: '操作',
          key: 'action',
          fixed: 'right',
          align: 'center',
          width: 120,
          render: (h, params) => {
            return h('div', [
              h('Button', {
                props: {
                  type: 'default',
                  size: 'large'
                }
              }, '删除用户')
            ])
          }
        }
      ],
      list: [
        {
          userId: 1,
          userName: 'bobo',
          name: '蔡敏波',
          gender: '男',
          telephone: '13750416301',
          email: '1535151019@qq.com',
          remark: ''
        },
        {
          userId: 1,
          userName: 'bobo',
          name: '蔡敏波',
          gender: '男',
          telephone: '13750416301',
          email: '1535151019@qq.com',
          remark: ''
        },
        {
          userId: 1,
          userName: 'bobo',
          name: '蔡敏波',
          gender: '男',
          telephone: '13750416301',
          email: '1535151019@qq.com',
          remark: ''
        },
        {
          userId: 1,
          userName: 'bobo',
          name: '蔡敏波',
          gender: '男',
          telephone: '13750416301',
          email: '1535151019@qq.com',
          remark: ''
        },
        {
          userId: 1,
          userName: 'bobo',
          name: '蔡敏波',
          gender: '男',
          telephone: '13750416301',
          email: '1535151019@qq.com',
          remark: ''
        },
        {
          userId: 1,
          userName: 'bobo',
          name: '蔡敏波',
          gender: '男',
          telephone: '13750416301',
          email: '1535151019@qq.com',
          remark: ''
        },
        {
          userId: 1,
          userName: 'bobo',
          name: '蔡敏波',
          gender: '男',
          telephone: '13750416301',
          email: '1535151019@qq.com',
          remark: ''
        },
        {
          userId: 1,
          userName: 'bobo',
          name: '蔡敏波',
          gender: '男',
          telephone: '13750416301',
          email: '1535151019@qq.com',
          remark: ''
        },
        {
          userId: 1,
          userName: 'bobo',
          name: '蔡敏波',
          gender: '男',
          telephone: '13750416301',
          email: '1535151019@qq.com',
          remark: ''
        },
        {
          userId: 1,
          userName: 'bobo',
          name: '蔡敏波',
          gender: '男',
          telephone: '13750416301',
          email: '1535151019@qq.com',
          remark: ''
        }
      ]
    }
  },
  methods: {

  },
  created () {

  },
  mounted () {

  }
}
</script>
<style lang="less">
.ivu-table th {
  font-size: 13px;
}
.ivu-table td {
  font-size: 13px;
}
.head {
  margin-bottom: 10px;
  text-align: right;
  font-size: 13px;
}
</style>
