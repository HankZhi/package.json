# package.json
我的package.json字段备注表
- :mortar_board: 官方相关
- :computer: 第三方相关

# 注释
```json
"module": "lib/esm/index.js"
```
> :computer: package.json中的module字段是gulp提出的，防止main入口commonjs与esm规范都有，专门用来表示esm的入口

```json
"sideEffects": false
```
> :computer: [深入理解sideEffects配置](https://libin1991.github.io/2019/05/01/%E6%B7%B1%E5%85%A5%E7%90%86%E8%A7%A3sideEffects%E9%85%8D%E7%BD%AE/)

```json
"typings": "lib/types/index.d.ts" or "types": "lib/types/index.d.ts"
```
> :computer: 主要用来描述该npm包的typescript类型主声明文件在什么位置，[声明文件的发布](https://www.tslang.cn/docs/handbook/declaration-files/publishing.html)

```json
"directories": {
  "lib": "lib",
  "test": "__tests__"
}
```
> :mortar_board: 描述项目目录信息

```json
"files": [
  "lib"
]
```
> :mortar_board: 描述npm包作为dependency安装时，应当输出哪些文件

