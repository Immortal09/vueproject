<template>
  <div >
    <div class="panel-primary ">
      <div class="panel-heading">
        <h3 class="panel-title">添加品牌</h3>
      </div>
    </div>
    <div>
      <label>id:<input type="text" class="form-control" placeholder="id">
      </label>
      <label>cname:<input type="text" class="form-control" placeholder="cname">
      </label>
      <button type="button" id="btn" class="btn btn-primary">查 询</button>
    </div>
    <table class="table table-bordered table-hover">
      <thead>
      <tr>
        <th>id</th>
        <th>name</th>
        <th>ctime</th>
        <th>description</th>
      </tr>
      </thead>
      <tbody>
      <tr v-for="item in this.cardata" :key="item.id">
        <td>{{item.id}}</td>
        <td>{{item.cname}}</td>
        <td>{{item.ctime}}</td>
        <td><a>{{item.decription}}</a></td>
      </tr>
      </tbody>
    </table>
  </div>
</template>

<script>
  $(function () {
    $("#btn").click(function () {
      alert("dadfa")
    })
  })
export default {
  name: 'HelloWorld',
  data () {
    return {
      cardata:[
        {id:1,cname:'宝马',ctime:new Date(),decription:'删除'},
        {id:2,cname:'大奔',ctime:new Date(),decription:'删除'},
        {id:3,cname:'玛莎拉蒂',ctime:new Date(),decription:'删除'}
      ]
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
