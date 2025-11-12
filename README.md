# StaticHub

`StaticHub` 是一个存储和管理静态文件（如 JSON 文件）的 GitHub 仓库。该仓库的目的是提供易于访问、共享和使用的数据文件。当前，仓库存储了一些静态数据文件，包括日历数据等，便于开发者或其他用户在项目中引用。

## 📂 目录结构

```
.
├── calendar/     # 📅 日历数据目录
│   └── 2025.json
└── README.md     # 项目说明文件
```

## 🧪 使用示例

### calendar

```jsonc
{
  // 政策文件网址
  "papers": ["*****"],
  "days": {
    "2025-01-01": {
      // 是否上班
      "workday": false,
      // 星期：1-7
      "weekday": 3
    }
  }
}
```

```
https://raw.githubusercontent.com/BaiZeLab/StaticHub/main/calendar/2025.json
```

```
https://cdn.jsdelivr.net/gh/BaiZeLab/StaticHub@main/calendar/2025.json
```

### proxifier

`ppx`文件采用了变量占位符的方式，满足多样化需求
ps: `.`需要进行转义`%2E`

```
https://vardelivr.alluniverse.vip/gh/BaiZeLab/StaticHub/main/proxifier/pac.ppx?address=localhost&port=21080
```
```
https://vardelivr.alluniverse.vip/gh/BaiZeLab/StaticHub/main/proxifier/pac.ppx?address=192%2E168%2E1%2E1&port=21080
```
