<p align="center">
  <img width="300" src="/src/assets/img/logo.png"/> <b>WebStarter</b>
</p>

<p align="center">
  <img src="https://svg.hamm.cn?key=Lang&value=TypeScript&bg=green"/>
  <img src="https://svg.hamm.cn?key=Base&value=Vue3"/>
  <img src="https://svg.hamm.cn?key=Build&value=Vite"/>
  <img src="https://svg.hamm.cn?key=UI&value=ElementPlus"/>
</p>


# AirPowerWebStarter

via [Github](https://github.com/HammCn/AirPowerWebStarter) / [Gitee](https://gitee.com/air-power/AirPowerWebStarter)

### 写在前面

你当前正在查看基于 `AirPower4T` 基础库的 宿主项目的代码, 我们使用的是 `Vite` 构建, 包管理使用的是 `yarn`,
请先安装前叙的相关工具后继续接下来的操作 ：）

- 安装 **TypeScript** :

  ```shell
  npm install -D typescript
  ```

### 一、初始化仓库

建议windows开发者使用 `git bash` 不要使用windows自带的拉垮的 `cmd` `powershell` 等。否则接下来的脚本可能出现问题，你只能通过自己手动去操作。

- 通过**Github**代码仓库初始化

  ```shell
  git clone https://github.com/HammCn/AirPowerWebStarter.git &&
  cd AirPowerWebStarter/src && 
  git clone https://github.com/HammCn/AirPower4T.git airpower && cd ../ &&
  yarn && cp .env.dev .env && yarn s
  ```


- 通过**Gitee**代码仓库初始化(推荐)

  ```shell
  git clone https://gitee.com/air-power/AirPowerWebStarter.git &&
  cd AirPowerWebStarter/src && 
  git clone https://gitee.com/air-power/AirPower4T.git airpower && cd ../ &&
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

启动项目前，我们建议你关闭 `visual studio code` 的 `Vetur` 插件，避免 `vue2` 和 `vue3` 产生冲突。

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

- Vue - Official
- ESLint
- SCSS Formatter

> 如碰到其他兼容问题，建议在工作区禁用以上三个插件之外的其他插件，特别是`Vetur`。

### 六、Enjoy your coding!
