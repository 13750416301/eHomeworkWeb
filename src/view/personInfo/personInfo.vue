<template>
  <div class="homework">
    <!-- <h1 style="text-align:center;margin-top:200px;color:#2d8cf0;font-size:50px;">STU学生作业系统</h1> -->
    <h1 style="color:#2d8cf0;margin:10px 0;">账户信息</h1>
    <Tabs value="info">
        <TabPane label="个人资料" name="info">
            <Form :model="formLeft" label-position="right" :label-width="100">
                <FormItem label="邮箱：">
                    <span class="item-value">1535151019@qq.com</span><Button type="default">修改</Button>
                </FormItem>
                <FormItem label="电话号码：">
                    <span class="item-value">13750416301</span><Button type="default">修改</Button>
                </FormItem>
                <FormItem label="姓名：">
                    <span class="item-value">蔡敏波</span><Button type="default">修改</Button>
                </FormItem>
                <FormItem label="性别：">
                    <RadioGroup style="font-size:14px;">
                        <Radio label="男">
                            <Icon type="md-male"></Icon>
                            <span class="item-value">男</span>
                        </Radio>
                        <Radio label="女">
                            <Icon type="md-female"></Icon>
                            <span class="item-value">女</span>
                        </Radio>
                    </RadioGroup>
                </FormItem>
                <FormItem label="学号：">
                    <span class="item-value">13750416301</span>
                </FormItem>
            </Form>
        </TabPane>
        <TabPane label="头像" name="avator">标签二的内容</TabPane>
        <TabPane label="密码" name="password">标签三的内容</TabPane>
        <TabPane label="登陆信息" name="loginLog">标签四的内容</TabPane>
    </Tabs>
  </div>
</template>

<script>
export default {
  name: 'homework',
  data () {
    return {
      inforCardData: [
        { title: '新增用户', icon: 'md-person-add', count: 803, color: '#2d8cf0' },
        { title: '累计点击', icon: 'md-locate', count: 232, color: '#19be6b' },
        { title: '新增问答', icon: 'md-help-circle', count: 142, color: '#ff9900' },
        { title: '分享统计', icon: 'md-share', count: 657, color: '#ed3f14' },
        { title: '新增互动', icon: 'md-chatbubbles', count: 12, color: '#E46CBB' },
        { title: '新增页面', icon: 'md-map', count: 14, color: '#9A66E4' }
      ],
      pieData: [
        { value: 335, name: '直接访问' },
        { value: 310, name: '邮件营销' },
        { value: 234, name: '联盟广告' },
        { value: 135, name: '视频广告' },
        { value: 1548, name: '搜索引擎' }
      ],
      barData: {
        Mon: 13253,
        Tue: 34235,
        Wed: 26321,
        Thu: 12340,
        Fri: 24643,
        Sat: 1322,
        Sun: 1324
      }
    }
  },
  mounted () {
    //
  }
}
</script>

<style lang="less" scoped>
/deep/ .ivu-tabs-tab {
    width: 100px;
    text-align: center;
    // padding: 0;
    // line-height: 45px;
    // font-size: 20px;
}
/deep/ .ivu-form-item {
    margin-bottom: 20px;
    padding-bottom: 15px;
    font-size: 14px;
    border-bottom: 1px dotted #000;
}
/deep/ .ivu-form .ivu-form-item-label {
    font-size: 14px;
    color: #000;
}
/deep/ .ivu-form-item-content {
    font-size: 14px;
    color: rgba(0, 0, 0, 0.5);
}
.item-value {
    margin-right: 20px;
    font-size: 14px;
}
</style>
