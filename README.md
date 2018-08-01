# webpack-demo
深入浅出webpack练习题

#### 1.webpack 安装
```
npm i -D webpack
```
#### 2.使用
```
node_modules/.bin/webpack
```
或添加npm scripts
```
"scripts": {
    "start": "webpack --config webpack.config.js"
}
sudo npm start
```
#### 3.输入输出配置
```
module.exports = {
  // JS 执行入口文件
  entry: './main.js',
  output: {
    // 把所有依赖的模块合并输出到一个 bundle.js 文件
    filename: 'bundle.js',
    // 输出文件都放到 dist 目录下
    path: path.resolve(__dirname, './dist'),
  }
};
```
