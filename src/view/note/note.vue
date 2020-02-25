<template>
  <div class="note">
    <!-- <h1 style="text-align:center;margin-top:200px;color:#2d8cf0;font-size:50px;">STU学生作业系统</h1> -->
    <div class="title">
        <div class="switchType">
            <Select v-model="model9" style="width:90px" placeholder="关注">
                <Option value="关注" label="关注"></Option>
                <Option value="推荐" label="推荐"></Option>
                <Option value="我的" label="我的"></Option>
                <Option value="特别关注" label="特别关注"></Option>
            </Select>
        </div>
        <div class="addNoteBtn">
            <Icon type="md-open" size="30" />
        </div>
    </div>
    <div class="gotoNote">
        <div class="gotoNoteTitle"><Icon type="md-bookmarks" style="color:#fff;margin-right:5px" size="20" />笔记本</div>
        <div class="arrow"><Icon type="ios-arrow-forward" /></div>
    </div>
    <div class="content">
        <div class="noContent">
            <div class="noContentImg">
                <img src="../../assets/images/note/noactivity.png" />
            </div>
            <p>暂无笔记</p>
        </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'note',
  data () {
    return {
      model9: ''
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
.title {
    position: relative;
    margin-bottom: 20px;
    .switchType {
        text-align: center;
    }
    .addNoteBtn {
        position: absolute;
        right: 40px;
        top: 0;
        cursor: pointer;
        color: #2d8cf0;
    }
}
.gotoNote {
    font-size: 15px;
    color: #fff;
    border-top: 2px solid #000;
    background-color: rgba(45, 140, 240, 0.8);
    height: 45px;
    line-height: 45px;
    padding: 0 40px;
    .gotoNoteTitle {
        float: left;
        display: flex;
        align-items: center;
    }
    .arrow {
        float: right;
    }
}
.content {
    margin-top: 100px;
    .noContent {
        text-align: center;
    }
}
</style>
