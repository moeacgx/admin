# Secondary Development / 二开说明

这个 fork 用来保存当前线上后台端的二开补丁，方便后续和 upstream 对照更新。

## 当前二开内容

1. 订单风控设置新增“邮箱域名黑名单”字段
2. 后台支持保存和展示该字段
3. 补充中英文本，方便管理端直接配置

## 本次主要改动文件

- `src/views/admin/components/SettingsOrderRiskControlTab.vue`
- `src/i18n/index.ts`

## 同步上游建议

```bash
git fetch upstream
git log --oneline upstream/main..origin/main
git diff upstream/main..origin/main
```
