<template>
  <div class="homeworkDetail">
    <h2 style="color:#2d8cf0;margin:10px 0;text-align:center;">马克思作业五</h2>
    <div class="homework-content">
      <Button class="exit-btn" type="default"><Icon type="md-power" style="margin-right:3px;" />退出作答</Button>
      <h3>一、<Icon type="ios-hand" color="#ff652f" size="20" style="margin-right:3px;" />单选题（50分）</h3>
      <div class="choice">
        <p class="choice-question">1、“人的理性为自然立法”的观点属于（）（10分）</p>
        <RadioGroup class="option" v-model="userAnswer[0]">
          <Radio label="A" class="radio">A.主观唯心主义</Radio>
          <Radio label="B" class="radio">B.唯物主义</Radio>
          <Radio label="C" class="radio">C.客观唯心主义</Radio>
          <Radio label="D" class="radio">D.形而上学的唯物主义</Radio>
        </RadioGroup>
        <p class="choice-question">2、“几十年的经验使我们深刻地认识到，学点哲学确实可以使人做事情少犯错误，做研究少走弯路。”下列观点与上述感悟相一致的是（）（10分）</p>
        <RadioGroup class="option" v-model="userAnswer[1]">
          <Radio label="A" class="radio">A.哲学是各门具体科学的基础</Radio>
          <Radio label="B" class="radio">B.哲学具有指导人们认识世界和改造世界的功能</Radio>
          <Radio label="C" class="radio">C.哲学是科学的世界观和方法论</Radio>
          <Radio label="D" class="radio">D.哲学是人们对某一领域规律的概括</Radio>
        </RadioGroup>
        <p class="choice-question">3、马克思主义产生于（）（10分）</p>
        <RadioGroup class="option" v-model="userAnswer[2]">
          <Radio label="A" class="radio">A.19世纪40年代</Radio>
          <Radio label="B" class="radio">B.18世纪40年代</Radio>
          <Radio label="C" class="radio">C.19世纪70年代</Radio>
          <Radio label="D" class="radio">D.18世纪70年代</Radio>
        </RadioGroup>
        <p class="choice-question">4、根据IID模型，开发过程中如果发现不能按期完成任务时应该（10分）</p>
        <RadioGroup class="option" v-model="userAnswer[3]">
          <Radio label="A" class="radio">A.增加开发人员</Radio>
          <Radio label="B" class="radio">B.开发人员加班加点争取完成任务</Radio>
          <Radio label="C" class="radio">C.取消或简化某些任务</Radio>
          <Radio label="D" class="radio">D.早期计划不周，发现问题时为期已晚，项目延期不可避免</Radio>
        </RadioGroup>
        <p class="choice-question">5、根据IID模型，开发过程中如果发现不能按期完成任务时应该（10分）</p>
        <RadioGroup class="option" v-model="userAnswer[4]">
          <Radio label="A" class="radio">A.增加开发人员</Radio>
          <Radio label="B" class="radio">B.开发人员加班加点争取完成任务</Radio>
          <Radio label="C" class="radio">C.取消或简化某些任务</Radio>
          <Radio label="D" class="radio">D.早期计划不周，发现问题时为期已晚，项目延期不可避免</Radio>
        </RadioGroup>
      </div>
      <h3>二、<Icon type="md-checkbox-outline" color="green" size="20" style="margin-right:3px;" />多选题（30分）</h3>
      <div class="choice">
        <p class="choice-question">1、根据IID模型，开发过程中如果发现不能按期完成任务时应该（10分）</p>
        <CheckboxGroup class="option" v-model="userAnswer2[0]">
          <Checkbox label="A" class="radio">A.增加开发人员</Checkbox>
          <Checkbox label="B" class="radio">B.开发人员加班加点争取完成任务</Checkbox>
          <Checkbox label="C" class="radio">C.取消或简化某些任务</Checkbox>
          <Checkbox label="D" class="radio">D.早期计划不周，发现问题时为期已晚，项目延期不可避免</Checkbox>
        </CheckboxGroup>
        <p class="choice-question">2、根据IID模型，开发过程中如果发现不能按期完成任务时应该（10分）</p>
        <CheckboxGroup class="option" v-model="userAnswer2[1]">
          <Checkbox label="A" class="radio">A.增加开发人员</Checkbox>
          <Checkbox label="B" class="radio">B.开发人员加班加点争取完成任务</Checkbox>
          <Checkbox label="C" class="radio">C.取消或简化某些任务</Checkbox>
          <Checkbox label="D" class="radio">D.早期计划不周，发现问题时为期已晚，项目延期不可避免</Checkbox>
        </CheckboxGroup>
        <p class="choice-question">3、根据IID模型，开发过程中如果发现不能按期完成任务时应该（10分）</p>
        <CheckboxGroup class="option" v-model="userAnswer2[2]">
          <Checkbox label="A" class="radio">A.增加开发人员</Checkbox>
          <Checkbox label="B" class="radio">B.开发人员加班加点争取完成任务</Checkbox>
          <Checkbox label="C" class="radio">C.取消或简化某些任务</Checkbox>
          <Checkbox label="D" class="radio">D.早期计划不周，发现问题时为期已晚，项目延期不可避免</Checkbox>
        </CheckboxGroup>
        <p class="choice-question">4、根据IID模型，开发过程中如果发现不能按期完成任务时应该（10分）</p>
        <CheckboxGroup class="option" v-model="userAnswer2[3]">
          <Checkbox label="A" class="radio">A.增加开发人员</Checkbox>
          <Checkbox label="B" class="radio">B.开发人员加班加点争取完成任务</Checkbox>
          <Checkbox label="C" class="radio">C.取消或简化某些任务</Checkbox>
          <Checkbox label="D" class="radio">D.早期计划不周，发现问题时为期已晚，项目延期不可避免</Checkbox>
        </CheckboxGroup>
        <p class="choice-question">5、我们可以从不同的角度理解马克思主义，包括（）（10分）</p>
        <CheckboxGroup class="option" v-model="userAnswer2[4]">
          <Checkbox label="A" class="radio">A.从创始者的认识成果讲，是马克思恩格斯创立的基本理论、基本观点、基本方法</Checkbox>
          <Checkbox label="B" class="radio">B.从阶级属性讲，是无产阶级争取自身解放和整个人类解放的科学理论</Checkbox>
          <Checkbox label="C" class="radio">C.从研究对象和主要内容讲，是无产阶级的世界观和方法论，是关于资本主义灭亡、社会主义胜利的科学理论</Checkbox>
          <Checkbox label="D" class="radio">D.从主要构成讲，包括马克思主义哲学、马克思主义政治经济学和科学社会主义</Checkbox>
        </CheckboxGroup>
      </div>
      <div class="shortAnswer">
        <h3>三、<Icon type="md-pricetags" color="blue" size="20" style="margin-right:3px;" />简答题（20分）</h3>
        <p class="shortAnswer-question">1、为什么说马克思主义哲学史是从大自然观到社会历史观的完备、彻底的唯物论？（10分）</p>
        <Input class="shortAnswer-ans" type="textarea" :rows="4" placeholder="请在框内输入你的答案……" />
        <p class="shortAnswer-question">2、什么是哲学的研究对象和哲学的基本问题？（10分）</p>
        <Input class="shortAnswer-ans" type="textarea" :rows="4" placeholder="请在框内输入你的答案……" />
      </div>
      <div class="submit-btn">
        <Button type="default" style="color:#fff;background-color:green;">提交作业</Button>
      </div>
    </div>
  </div>
</template>
<script>
// import moment from 'moment'
// import axios from 'axios'
export default {
  name: 'homeworkDetail',
  created () {
  },
  data () {
    return {
      userAnswer: [1, 2, 3, 4, 5],
      userAnswer2: [1, 2, 3, 4, 5],
      homeworkData: [
        {
          title: '马克思作业五',
          publisher: '杨沐',
          beginTime: '2020年2月25日20点33分',
          endTime: '2020年2月25日20点33分',
          status: '进行中'
        },
        {
          title: '马克思作业五',
          publisher: '杨沐',
          beginTime: '2020年2月25日20点33分',
          endTime: '2020年2月25日20点33分',
          status: '进行中'
        },
        {
          title: '马克思作业五',
          publisher: '杨沐',
          beginTime: '2020年2月25日20点33分',
          endTime: '2020年2月25日20点33分',
          status: '进行中'
        },
        {
          title: '马克思作业五',
          publisher: '杨沐',
          beginTime: '2020年2月25日20点33分',
          endTime: '2020年2月25日20点33分',
          status: '进行中'
        },
        {
          title: '马克思作业五',
          publisher: '杨沐',
          beginTime: '2020年2月25日20点33分',
          endTime: '2020年2月25日20点33分',
          status: '进行中'
        }
      ]
    }
  },
  methods: {
    view () {
      console.log('view')
    }
  },
  mounted () {
    //
  }
}
</script>

<style lang="less" scoped>
.homework-content {
  width: 100%;
  height: 350px;
  padding-top: 15px;
  border-top: 1px solid rgba(0, 0, 0, 0.5);
  .exit-btn {
    right: 35px;
    top: 90px;
    position: fixed;
    color: #fff;
    background-color: rgba(255, 0, 0, 0.5);
  }
}
.choice {
  width: 100%;
  .choice-question {
    margin-top: 10px;
  }
  .option {
    margin-top: 8px;
    .radio {
      display: block;
      margin-bottom: 8px;
    }
  }
}
.shortAnswer {
  width: 100%;
  .shortAnswer-question {
    margin-top: 10px;
  }
  .shortAnswer-ans {
    margin-top: 8px;
  }
}
.submit-btn {
  width: 100%;
  height: auto;
  margin-top: 10px;
  text-align: center;
}
</style>
