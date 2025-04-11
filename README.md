# bossjob-doc
doc of bossjob

## bossjob网址大全

> bossjob-jobseeker-client【求职端】【prod】https://bossjob.com

> bossjob-jobseeker-client【求职端】【test】https://demo.bossjob.com

> bossjob-jobseeker-client【求职端】【test2】https://test2demo.bossjob.com

> Bosshunt-Client【雇主端】【prod】https://employer.bossjob.com

> Bosshunt-Client【雇主端】【test】https://dev.employer.bossjob.com

> Bosshunt-Client【雇主端】【test2】https://test2.employer.bossjob.com

## 富文本编辑器

### react-quill实现有序列表始终正确排序

```
.ql-editor {
  counter-reset: global-list; /* 全局计数器 */
}
.ql-editor ol li {
  counter-increment: global-list; /* 递增全局计数器 */
}
.ql-editor ol li:before {
  content: counter(global-list, decimal) '. ';
}
```

## white-space换行

| 属性值      | 保留空格/换行      | 自动换行 | 行为说明                                 |
|-------------|-------------------|----------|----------------------------------------|
| `normal`    | ❌                | ✅       | 默认行为：合并连续空格，忽略换行符，自动换行      |
| `pre`       | ✅                | ❌       | 严格保留所有空格和换行符，文本可能溢出容器       |
| `pre-wrap`  | ✅                | ✅       | 保留空格和换行符，但自动换行避免溢出（推荐属性）   |
| `pre-line`  | ❌（仅保留换行符） | ✅       | 合并连续空格，保留换行符，自动换行            |

white-space: pre-wrap; 是 pre 和 normal 的混合体：
✅ ​保留格式 + ✅ ​响应式换行 = 兼顾代码可读性与页面适配性。


