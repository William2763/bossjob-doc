# bossjob-doc
doc of bossjob

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
