# 考拉 js 标准
本标准基于 [eslint-config-standard](https://github.com/standard/eslint-config-standard)

```json
{
  "env": {
    "mocha": true,
    "es6": true,
    "node": true
  },
  "extends": "standard",
  "plugins": [
    "standard"
  ]
}
```


## Install

安装配置包

```bash
npm install --save-dev eslint-config-klg eslint-config-standard
```

因为 eslint 的插件独立于 config 之外的设计，你还必须手动安装以下插件


```bash
npm install --save-dev eslint-plugin-standard eslint-plugin-promise eslint-plugin-import eslint-plugin-node
```

## 配置
编辑 .eslintrc 加入即可

```.eslintrc
{
  "extends": "eslint-config-klg"，
  "rules": {}
}
```

## 注意事项
eslint 的插件安装位置要和 eslint 的安装位置保持一致，如果 eslint 是 global 的，那么插件也需要是 global 的。