---
sidebar_position: 1
---

# 安装

import Tabs from '@theme/Tabs';
import TabItem from '@theme/TabItem';

:::tip 使用者提示

V3用户可阅读此文档进行体验，开发者请阅读后续教程

:::

- 安装源码

> 请在合适目录中执行，确保具有合理的权限

<Tabs>
  <TabItem value="16" label="Gitee" default>

```sh
git clone --depth=1 https://github.com/yoimiya-kokomi/Miao-Yunzai.git
cd Miao-Yunzai
git clone --depth=1 https://github.com/yoimiya-kokomi/miao-plugin.git ./plugins/miao-plugin/
```

  </TabItem>
  <TabItem value="18" label="Github" default>

```sh
git clone --depth=1 https://gitee.com/yoimiya-kokomi/Miao-Yunzai.git
cd Miao-Yunzai
git clone --depth=1 https://gitee.com/yoimiya-kokomi/miao-plugin.git ./plugins/miao-plugin/
```

  </TabItem>
</Tabs>

- 进入目录

```sh
cd yunzaijs
```

- 安装依赖

```sh
# 国内镜像，已安装可忽视
npm config set registry https://registry.npmmirror.com
```

> 不推荐npm、pnpm、cnpm等

```sh
# yarn 不能使用2.x版本
npm install yarn@1.19.1 -g
```

<Tabs>
  <TabItem value="16" label="node>=18" default>

> 如果 node < 18 需要加参数 `--ignore-engines`

```sh
yarn
```

  </TabItem>
  <TabItem value="18" label="node<18" default>

```sh
yarn --ignore-engines
```

  </TabItem>
</Tabs>

- 启动

```sh
yarn app
```

- 重新登录

```sh
yarn login
```

- 进程托管

```sh
yarn start
```

> 更多内容，请阅读 [PM2](https://pm2.keymetrics.io/) 使用文档
