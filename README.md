# zyrthi-registry

zyrthi 平台索引仓库。

## 用途

记录所有已注册的平台仓库地址，供 `zyrthi platform install` 查询使用。

## 索引格式

```yaml
platforms:
  <platform-name>:
    name: 显示名称
    description: 描述
    vendor: 厂商
    repository: 仓库地址
    chips:
      - 支持的芯片列表
```

## 注册新平台

1. Fork 本仓库
2. 编辑 `index.yaml`，添加新平台
3. 提交 PR

## 平台仓库要求

平台仓库必须包含：
- `platform.yaml` — 平台配置
- `releases/` — 烧录插件（或 GitHub Release）
