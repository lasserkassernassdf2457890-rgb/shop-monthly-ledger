# 店铺月账

用抖店导出的订单、售后、资金流水和寄件明细做月结。按店铺实际情况加入 SKU 成本、1688 采购、千川消耗和月度费用，生成经营汇总、逐单对账明细和待核实清单。

## 安装到 Codex

1. 在 Codex 打开用于月结的本地项目。
2. 把 [v0.1.0 安装包下载链接](https://github.com/lasserkassernassdf2457890-rgb/shop-monthly-ledger/releases/download/v0.1.0/doudian-month-close-v0.1.0.zip) 发给 Codex，输入「请下载这个 ZIP，把里面的 `doudian-month-close` 文件夹解压到当前项目的 `.agents/skills/`」。也可以下载后手动解压到同一目录。
3. 安装后发「用店铺月账带我跑一遍演示」，正式核算时再提供自己的报表和店铺规则。

有 Node.js 22.20 或更新版本的用户，可在项目目录执行下面的命令安装。

```powershell
npx skills@1.9.0 add "https://github.com/lasserkassernassdf2457890-rgb/shop-monthly-ledger/releases/download/v0.1.0/doudian-month-close-v0.1.0.zip" -a codex --copy
```

核算脚本需要 Python 3.10 或更新版本。读取 XLSX 报表还需要 `openpyxl`。已导出的报表可直接用来核算，需要协助导表时可使用 Ego 浏览器，并在对应平台登录。

## 开始月结

在 Codex 输入「用店铺月账核算这家抖店的月度经营盈亏」，按提示提供月份、核对截止日和报表。首次向导会确认发货方式、采购成本和适用的费用规则。以后可沿用同一家店的配置。核算结果和待核实事项保存在本地。
