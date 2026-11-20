# 使用示例

以下词汇均为说明功能的示例，不对应任何个人学习记录。

## 1. 整理含音标和词性的文本

输入：

```text
library /ˈlaɪbrəri/ n. 图书馆
helpful /ˈhelpfəl/ adj. 有帮助的
take part in 参加
```

预期词表：

| 英文 | 中文 |
| :---: | :--- |
| library | 图书馆 |
| helpful | 有帮助的 |
| take part in | 参加 |

## 2. 纠正拼写与补充释义

输入：

```text
neccessary 必要的
go aborad 出国
reliable
```

预期词表：

| 英文 | 中文 |
| :---: | :--- |
| necessary | 必要的 |
| go abroad | 出国 |
| reliable | 可靠的 |

对话反馈中应说明 `neccessary → necessary`、`go aborad → go abroad`，而非将原错误拼写写到文档中。

## 3. 连续追加

先发送两条词汇，再在同一任务发送另一组：

```text
prepare 准备
improve 提高、改善
```

下一条消息：

```text
progress 进步
```

预期：原有两条不被覆盖；`progress` 填入第三个空行。若本页已满，下一页使用同样表格格式。

## 4. 照片输入

拍摄手写词汇列表或上传教材截图，然后说「整理这些单词」。应按阅读顺序提取词汇，忽略音标及词性。对于模糊不清的词，应提示待确认，不应凭空补写。

## 5. 指定已有文档

示例请求：「把下面的词汇追加到我指定的 Google Docs 文档的『Unit 3』标签页。」

提供可访问的文档链接后，技能应只修改指定标签页并保留原有词表内容。如果无法访问，则停止写入并说明问题。
