<template>
  <div id="collect3">
    <div id="head3">
      <tr>
        <th id="MyCollectFont3">
          最近浏览
          <i class="el-icon-time"></i>
        </th>
        <th id="CollectTime3">
          修改时间
        </th>
      </tr>
    </div>
    <tr id="line3">
      <td>
        <hr size="1px" color="#CFCFCF" width="100%"/>
      </td>
    </tr>
    <div id="body3" >
      <div id="body-row3" v-for="file in files" :key="file.name">
        <div id="blank15"><a href="" >{{ file.name }}</a></div>
        <div id="blank16">{{ file.time }}</div>
        <div id="blank17"><a href="" @click="delFile">删除记录</a></div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name:"create",
  data: function () {
    return {
      files:[
        {name:"这是一个示例文档", writter:"李书实", time:"2020-08-12"},
        {name:"这是一个示例文档", writter:"李书实", time:"2020-08-12"},
        {name:"这是一个示例文档有很长的标题，没错很长的标题", writter:"李书实", time:"2020-08-12"},
        {name:"这是一个示例文档", writter:"李书实", time:"2020-08-12"},
        {name:"这是一个示例文档", writter:"李书实", time:"2020-08-12"},
        {name:"这是一个示例文档有很长的标题，没错很长的标题", writter:"李书实", time:"2020-08-12"},
        {name:"这是一个示例文档", writter:"李书实", time:"2020-08-12"},
        {name:"这是一个示例文档", writter:"李书实", time:"2020-08-12"},
        {name:"这是一个示例文档有很长的标题，没错很长的标题", writter:"李书实", time:"2020-08-12"},
        {name:"这是一个示例文档", writter:"李书实", time:"2020-08-12"},
        {name:"这是一个示例文档", writter:"李书实", time:"2020-08-12"},
        {name:"这是一个示例文档有很长的标题，没错很长的标题", writter:"李书实", time:"2020-08-12"},
        {name:"这是一个示例文档", writter:"李书实", time:"2020-08-12"},
      ]
    }
  },
  methods: {
    delFile: function() {
      
    }
  }
}
</script>

<style>
a:hover {color: #54A193}

a:link {color: #FFFFFF}

a {
  color: #616161;
  text-decoration: none;
}

.file-name {
  color: #616161;
  text-decoration: none;
}
.file-name:hover {
  cursor: pointer;
  color: #54A193
}
#collect3 {
  position: absolute;
  left:17.6vw;
  bottom: 0;
  width: 62.5vw;
  height: calc(100vh - 68px);
  background-color: rgba(242, 244, 244, 1);
}
#head3{
  position: absolute;
  bottom: 91%;
  left: 10%;
}
#MyCollectFont3{
  height: 40px;
  font-family: "Hiragino Sans GB", "Microsoft YaHei", "微软雅黑",
  "Neue Haas Grotesk", "Helvetica Neue", Helvetica, Arial, sans-serif;
  font-style: normal;
  font-weight: normal;
  font-size: 28px;
  line-height: 37px;
  color: #616161;
}

#CollectTime3{
  position: relative;
  width: 60%;
  height: 60%;
  left: 75%;
  top: 50%;
  font-family: "Hiragino Sans GB", "Microsoft YaHei", "微软雅黑",
  "Neue Haas Grotesk", "Helvetica Neue", Helvetica, Arial, sans-serif;
  font-style: normal;
  font-weight: normal;
  font-size: 20px;
  line-height: 26px;
  color: #CFCFCF;
}

#line3{
  position: absolute;
  width: 80%;
  height: 0;
  left: 10%;
  bottom: 89%;
  border: 0.2px solid #CFCFCF;
}

#body3{
  position: absolute;
  height: 85%;
  width: 80%;
  left: 10%;
  top:13%;
  overflow-y: auto;
  overflow-x: hidden ;
  bottom: 0;
}
#body-row3 {
  position: relative;
  top:1%;
  height: 8%;
  valign: bottom;
}

#blank15 {
  width: 50%;
  height: 100%;
  font-family: "Hiragino Sans GB", "Microsoft YaHei", "微软雅黑",
  "Neue Haas Grotesk", "Helvetica Neue", Helvetica, Arial, sans-serif;
  font-style: normal;
  font-weight: normal;
  font-size: 25px;
  line-height: 33px;
  color: #616161;
  overflow: hidden;
  text-overflow: ellipsis;
  white-space: nowrap;
  text-align: left;
}

#blank16 {
  position: absolute;
  height: 100%;
  left: 64%;
  margin-top: -5%;
  font-family: "Hiragino Sans GB", "Microsoft YaHei", "微软雅黑",
  "Neue Haas Grotesk", "Helvetica Neue", Helvetica, Arial, sans-serif;
  font-style: normal;
  font-weight: normal;
  font-size: 20px;
  line-height: 26px;
  color: #616161;
  overflow: hidden;
  text-overflow: ellipsis;
  white-space: nowrap;
  text-align: left;
  float: left;
}

#blank17 {
  position: absolute;
  height: 100%;
  left: 85%;
  margin-top: -5%;
  font-family: "Hiragino Sans GB", "Microsoft YaHei", "微软雅黑",
  "Neue Haas Grotesk", "Helvetica Neue", Helvetica, Arial, sans-serif;
  font-style: normal;
  font-weight: normal;
  font-size: 20px;
  line-height: 26px;
  color: #616161;
  overflow: hidden;
  text-overflow: ellipsis;
  white-space: nowrap;
  text-align: left;
  float: left;
}
</style>
