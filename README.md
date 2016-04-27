# webpack_diary
webpack学习日志


webpack #最基本的启动webpack命令

webpack -w   #提供watch方法，实时进行打包更新
  
webpack -p  #对打包后的文件进行压缩

webpack -d  #提供SourceMaps，方便调试

webpack --colors  #输出结果带彩色，比如：会用红色显示耗时较长的步骤

webpack --profile  #输出性能数据，可以看到每一步的耗时

webpack --display-modules  #默认情况下 node_modules 下的模块会被隐藏，加上这个参数可以显示这些被隐藏的模块

	

主要目录结构
- webapp/               # webapp根目录
- src/                # 开发目录
  + css/              # css资源目录
  + img/              # webapp图片资源目录
  - js/               # webapp js&jsx资源目录
    - components/     # 标准组件存放目录
        - foo/        # 组件foo
          + css/      # 组件foo的样式
          + js/       # 组件foo的逻辑
          + tmpl/     # 组件foo的模板
          index.js    # 组件foo的入口
        + bar/        # 组件bar
    + lib/            # 第三方纯js库
    ...               # 根据项目需要任意添加的代码目录
  + tmpl/             # webapp前端模板资源目录
  a.html              # webapp入口文件a
  b.html              # webapp入口文件b
- assets/             # 编译输出目录，即发布目录
  + js/               # 编译输出的js目录
  + img/              # 编译输出的图片目录
  + css/              # 编译输出的css目录
  a.html              # 编译输出的入口a
  b.html              # 编译处理后的入口b
+ mock/               # 假数据目录
app.js                # 本地server入口
routes.js             # 本地路由配置
webpack.config.js     # webpack配置文件
gulpfile.js           # gulp任务配置
package.json          # 项目配置
README.md             # 项目说明
