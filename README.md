# Demo宿主项目

### 写在前面

你当前正在查看基于 ```AirPower``` 基础库的 DEMO宿主项目的代码, 我们使用的是 ```Vite``` 构建, 包管理使用的是 ```yarn```, 请先安装前叙的相关工具后继续接下来的操作 ：）

### 一、初始化仓库

> 建议windows开发者使用 ```git bash``` 不要使用windows自带的拉垮的 ```cmd``` ```powershell``` 等。否则接下来的脚本可能出现问题，你只能通过自己手动去操作。

任选一个方式的脚本一键初始化项目

- ssh方式
```shell
git clone git@github.com:HammCn/AirPowerWebDemo.git &&
cd AirPowerDemo/src && 
git clone git@github.com:HammCn/AirPower4T.git airpower && cd ../ &&
yarn && cp .env.dev .env && yarn s
```

- https方式
```shell
git clone https://github.com/HammCn/AirPowerWebDemo.git &&
cd AirPowerDemo/src && 
git clone https://github.com/HammCn/AirPower4T.git airpower && cd ../ &&
yarn && cp .env.dev .env && yarn s
```

### 二、修改环境变量

按需修改配置
```conf
VITE_APP_NAME = "开发环境"
VITE_APP_API_URL = "/api/"
VITE_APP_STATIC_URL = "/static/"
```

### 三、启动和打包

启动项目前，我们建议你关闭 ```visual studio code``` 的 ```Vetur``` 插件，避免 ```vue2``` 和 ```vue3``` 产生冲突。


```shell
# 启动项目
yarn s              #缩写指令

# 打包项目
yarn dev            #开发环境 使用.env.dev
yarn test           #测试环境 使用.env.test
yarn production     #生产环境 使用.env.production
```

### 四、其他命令

```shell
#使用标准commit模板
yarn c   

#更新项目和AirPower
yarn u   

#查看Git格式化日志
yarn l           
```

### 五、推荐的VSCODE插件扩展

- TypeScript Vue Plugin (Volar)
- Vue Language Features (Volar)
- ESLint
- SCSS Formatter

> 如碰到其他兼容问题，建议在工作区禁用以上四个插件之外的其他插件，特别是```Vetur```。

### And now, enjoy your coding!