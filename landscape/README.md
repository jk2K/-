# 使用指南

产品入选标准，满足以下任一条件即可
1. MMR 大于 2000 万人民币
2. 客户数量超过 200 家
3. 完成 B 轮融资

logo 要求
1. svg 格式，如果是 png 格式，可以先去 figma 上进行转换

安装 landscape2
```bash
# 如果 cargo 没有安装过，可以参考 https://doc.rust-lang.org/cargo/getting-started/installation.html#install-rust-and-cargo 安装
git clone https://github.com/jk2K/landscape2.git
cargo install --path landscape2
```

编译网站
```bash
landscape2 build \
  --data-file data.yml \
  --settings-file settings.yml \
  --guide-file guide.yml \
  --logos-path logos \
  --output-dir build
```

本地预览网站
```bash
landscape2 serve --landscape-dir build
```
