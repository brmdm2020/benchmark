好的，作为一名资深的代码工程师，我为你准备了一份详尽的 GitHub Flavored Markdown (GFM) 语法测试大全。这份文件旨在全面覆盖 GFM 的各种语法特性，你可以直接将其内容复制到 GitHub 的 `.md` 文件中查看效果。

---

# GitHub Flavored Markdown (GFM) 语法测试大全

这是一份全面的 GFM 语法测试文件，旨在展示和测试 GitHub Flavored Markdown 的各种功能。

## 目录
1.  基础语法 [<sup>1</sup>](#基础语法)
    *   标题 [<sup>2</sup>](#标题)
    *   段落和换行 [<sup>3</sup>](#段落和换行)
    *   文本样式 [<sup>4</sup>](#文本样式)
    *   引用块 [<sup>5</sup>](#引用块)
    *   列表 [<sup>6</sup>](#列表)
    *   水平分割线 [<sup>7</sup>](#水平分割线)
2.  代码 [<sup>8</sup>](#代码)
    *   行内代码 [<sup>9</sup>](#行内代码)
    *   代码块 [<sup>10</sup>](#代码块)
3.  链接和图片 [<sup>11</sup>](#链接和图片)
    *   链接 [<sup>12</sup>](#链接)
    *   图片 [<sup>13</sup>](#图片)
4.  GFM 扩展语法 [<sup>14</sup>](#gfm-扩展语法)
    *   表格 [<sup>15</sup>](#表格)
    *   任务列表 [<sup>16</sup>](#任务列表)
    *   提及 (Mentions) [<sup>17</sup>](#提及-mentions)
    *   议题和拉取请求引用 [<sup>18</sup>](#议题和拉取请求引用)
    *   Emoji [<sup>19</sup>](#emoji)
    *   脚注 [<sup>20</sup>](#脚注)
    *   警告框 (Alerts) [<sup>21</sup>](#警告框-alerts)
    *   折叠内容 [<sup>22</sup>](#折叠内容)
    *   数学表达式 [<sup>23</sup>](#数学表达式)
    *   HTML [<sup>24</sup>](#html)

---

## 基础语法

### 标题

```markdown
# 这是一级标题 (H1)
## 这是二级标题 (H2)
### 这是三级标题 (H3)
#### 这是四级标题 (H4)
##### 这是五级标题 (H5)
###### 这是六级标题 (H6)
```

### 段落和换行

这是一个段落。段落之间由一个或多个空行分隔。

如果想在段落内强制换行，
可以在行尾添加两个或更多的空格，
或者直接使用 HTML 的 `<br>` 标签。

### 文本样式

```markdown
*斜体文本*
_斜体文本_

**粗体文本**
__粗体文本__

***粗斜体文本***
___粗斜体文本___

~~删除线文本~~

`行内代码` 是用反引号包围的。

上标: X<sup>2</sup>
下标: H<sub>2</sub>O
```

**效果:**

*斜体文本*
_斜体文本_

**粗体文本**
__粗体文本__

***粗斜体文本***
___粗斜体文本___

~~删除线文本~~

`行内代码` 是用反引号包围的。

上标: X<sup>2</sup>
下标: H<sub>2</sub>O

### 引用块

可以使用 `>` 符号来创建引用块。

```markdown
> 这是一个引用块。
>
> > 这是一个嵌套的引用块。
> >
> > > 更深层次的嵌套。
>
> ### 引用块内也可以包含其他 Markdown 元素
>
> *   列表项 1
> *   列表项 2
```

**效果:**

> 这是一个引用块。
>
> > 这是一个嵌套的引用块。
> >
> > > 更深层次的嵌套。
>
> ### 引用块内也可以包含其他 Markdown 元素
>
> *   列表项 1
> *   列表项 2

### 列表

#### 无序列表

使用 `*`, `+`, 或 `-` 来创建无序列表。

```markdown
* 列表项 1
* 列表项 2
  * 嵌套列表项 2.1
  * 嵌套列表项 2.2
- 列表项 3
+ 列表项 4
```

**效果:**

*   列表项 1
*   列表项 2
    *   嵌套列表项 2.1
    *   嵌套列表项 2.2
*   列表项 3
*   列表项 4

#### 有序列表

使用数字加 `.` 来创建有序列表。

```markdown
1. 第一个项目
2. 第二个项目
   1. 嵌套项目 2.1
   2. 嵌套项目 2.2
3. 第三个项目
```

**效果:**

1.  第一个项目
2.  第二个项目
    1.  嵌套项目 2.1
    2.  嵌套项目 2.2
3.  第三个项目

### 水平分割线

使用三个或更多的 `---`, `***`, 或 `___` 来创建水平分割线。

```markdown
---
***
___
```

**效果:**

---

***

___

## 代码

### 行内代码

使用单个反引号 `` ` `` 包围代码。

```markdown
这是一个包含 `console.log("Hello, World!");` 的句子。
```

**效果:**

这是一个包含 `console.log("Hello, World!");` 的句子。

### 代码块

使用三个反引号 ` ``` ` 来创建代码块，并可以指定语言以实现语法高亮。 [1]

````markdown
```javascript
// Javascript 代码示例
function greet(name) {
  console.log(`Hello, ${name}!`);
}

greet('GitHub');
```

```python
# Python 代码示例
def add(a, b):
  return a + b

print(add(5, 3))
```

```diff
- 删除的行
+ 添加的行
```````

**效果:**

```javascript
// Javascript 代码示例
function greet(name) {
  console.log(`Hello, ${name}!`);
}

greet('GitHub');
```

```python
# Python 代码示例
def add(a, b):
  return a + b

print(add(5, 3))
```

```diff
- 删除的行
+ 添加的行
```

## 链接和图片

### 链接

```markdown
<!-- 内联链接 -->
GitHub 官网 [<sup>25</sup>](https://github.com "GitHub 的 Title")

<!-- 引用样式链接 -->
[GitHub] 是一个代码托管平台。

: https://github.com/

<!-- 自动链接 -->
<https://github.com>
```

**效果:**

GitHub 官网 [<sup>25</sup>](https://github.com "GitHub 的 Title")

[GitHub][1] 是一个代码托管平台。

<https://github.com>

[1]: https://github.com/

### 图片

```markdown
<!-- 内联图片 -->
!GitHub Logo [<sup>26</sup>](https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png "GitHub Logo")

<!-- 带链接的图片 -->
![GitHub Logo [<sup>26</sup>](https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png "GitHub Logo")](https://github.com)
```

**效果:**

!GitHub Logo [<sup>26</sup>](https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png "GitHub Logo")

![GitHub Logo [<sup>26</sup>](https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png "GitHub Logo")](https://github.com)

## GFM 扩展语法

### 表格

使用 `|` 和 `-` 来创建表格。使用 `:` 来控制对齐方式。

```markdown
| 左对齐 | 居中对齐 | 右对齐 |
| :--- | :---: | ---: |
| 单元格 1 | 单元格 2 | 单元格 3 |
| 单元格 4 | 单元格 5 | 单元格 6 |
| 这是一个比较长的内容 | a | b |
```

**效果:**

| 左对齐              | 居中对齐 | 右对齐 |
| :-------------------- | :------: | -----: |
| 单元格 1              | 单元格 2 | 单元格 3 |
| 单元格 4              | 单元格 5 | 单元格 6 |
| 这是一个比较长的内容 | a        | b      |

### 任务列表

在列表项前加上 `[ ]` 或 `[x]`。

```markdown
- [x] 完成 GFM 语法测试大全的编写
- [ ] 学习更多关于 Markdown 的知识
- [ ] 部署一个新的项目
  - [x] 完成项目初始化
  - [ ] 编写核心代码
```

**效果:**

- [x] 完成 GFM 语法测试大全的编写
- [ ] 学习更多关于 Markdown 的知识
- [ ] 部署一个新的项目
  - [x] 完成项目初始化
  - [ ] 编写核心代码

### 提及 (Mentions)

可以直接 @ 某个用户或团队。

```markdown
@github, 这是一个很棒的功能！
```

**效果:** (在 GitHub 环境下会高亮并通知相关用户)
@github, 这是一个很棒的功能！

### 议题和拉取请求引用

可以直接引用仓库内的议题（Issue）或拉取请求（Pull Request）。

```markdown
修复了 #123 中提到的 bug。
```

**效果:** (在 GitHub 仓库中会自动转换为指向该 Issue 的链接)
修复了 #123 中提到的 bug。

### Emoji

可以直接使用 `:emoji_name:` 的形式插入 Emoji。

```markdown
:tada: :rocket: :sparkles: :octocat:
```

**效果:**

🎉 🚀 ✨ 🐙

### 脚注

使用 `[^标识]` 来创建脚注。

```markdown
这是一个需要脚注的句子。[^1]
这是另一个需要脚注的句子。[^note]

[^1]: 这是第一个脚注的详细内容。
[^note]: 这是另一个脚注的详细内容，可以使用非数字标识。
```

**效果:**

这是一个需要脚注的句子。[^1]
这是另一个需要脚注的句子。[^note]

[^1]: 这是第一个脚注的详细内容。
[^note]: 这是另一个脚注的详细内容，可以使用非数字标识。

### 警告框 (Alerts)

这是 GFM 新增的特性，用于创建不同类型的提示信息。 [1]

```markdown
> [!NOTE]
> 这是一个提示信息。

> [!TIP]
> 这是一个小技巧。

> [!IMPORTANT]
> 这是重要的信息。

> [!WARNING]
> 这是一个警告信息。

> [!CAUTION]
> 这是一个需要谨慎操作的信息。
```

**效果:**

> [!NOTE]
> 这是一个提示信息。

> [!TIP]
> 这是一个小技巧。

> [!IMPORTANT]
> 这是重要的信息。

> [!WARNING]
> 这是一个警告信息。

> [!CAUTION]
> 这是一个需要谨慎操作的信息。

### 折叠内容

使用 `<details>` 和 `<summary>` HTML 标签来创建可折叠的内容区域。

```markdown
<details>
<summary>点击这里展开详细内容</summary>

这里是隐藏的详细内容，可以包含任何 Markdown 语法。

- 列表项
- `代码`
- **粗体**

</details>
```

**效果:**

<details>
<summary>点击这里展开详细内容</summary>

这里是隐藏的详细内容，可以包含任何 Markdown 语法。

- 列表项
- `代码`
- **粗体**

</details>

### 数学表达式

GFM 支持使用 KaTeX 来渲染数学公式。 [1]

````markdown
行内公式使用 `$` 包围： $E=mc^2$

块级公式使用 `$$` 包围：
$$
\frac{\partial u}{\partial t} = h^2 \left( \frac{\partial^2 u}{\partial x^2} + \frac{\partial^2 u}{\partial y^2} + \frac{\partial^2 u}{\partial z^2} \right)
$$

或者使用 ` ```math ` 代码块：
```math
\int_0^\infty e^{-x^2} dx = \frac{\sqrt{\pi}}{2}
```
````

**效果:**

行内公式使用 `$` 包围： $E=mc^2$

块级公式使用 `$$` 包围：
$$
\frac{\partial u}{\partial t} = h^2 \left( \frac{\partial^2 u}{\partial x^2} + \frac{\partial^2 u}{\partial y^2} + \frac{\partial^2 u}{\partial z^2} \right)
$$

或者使用 ` ```math ` 代码块：
```math
\int_0^\infty e^{-x^2} dx = \frac{\sqrt{\pi}}{2}
```

### HTML

GFM 支持内联 HTML。

```html
<!-- 你可以直接在 Markdown 中使用 HTML 标签 -->
<p style="color:red;">这是一个红色的段落。</p>

<div>
  <h3>HTML 块级元素</h3>
  <p>这是一个 div 容器内的段落。</p>
</div>
```

**效果:**

<!-- 你可以直接在 Markdown 中使用 HTML 标签 -->
<p style="color:red;">这是一个红色的段落。</p>

<div>
  <h3>HTML 块级元素</h3>
  <p>这是一个 div 容器内的段落。</p>
</div>

---
