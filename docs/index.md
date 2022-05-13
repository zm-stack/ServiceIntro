# 智能合约安全审计服务介绍

*<p align="right">by. 北京大学信息安全实验室</p>*

## 项目简介  

&emsp;&emsp;传统软件漏洞检测技术难以支持区块链智能合约的安全审计，无法识别由于智能合约语义错误或漏洞导致的安全风险和合约交易损失。  
&emsp;&emsp;本项目重点研究智能合约安全审计问题，涉及基于污点分析技术的已知智能合约漏洞检测、基于深度学习及语义分析技术的未知智能合约漏洞挖掘，和适用于组合交易的智能合约形式化验证方法。突破现有智能合约在漏洞检测、漏洞挖掘、功能验证技术在分析精度、处理规模和应用场景上的局限性。  
&emsp;&emsp;目前，本项目团队基于上述关键技术的研究工作已取得多项专利及论文成果并发现以太坊平台多个中高危智能合约零日漏洞。基于该理论框架实现的智能合约安全审计工具集，有效实现对合约安全风险的检测、定位、异常诊断功能，为保障高并发环境下智能合约的可信、可靠提供理论基础和技术支撑。

## <center>智能合约漏洞检测</center>

&emsp;&emsp;本项目支持针对Ethereum系统solidity智能合约和Hyperledger Fabric系统Go链码的已知安全漏洞的检测和定位。

### 针对solidity智能合约

覆盖漏洞如下：
|  序号  |  漏洞名称  |  说明  |
|:-------------|:------------------|:------|
|  1  |  溢出  |  未受保护的数值计算  |
|  2  |  重入  |  函数内和函数间重入攻击  |
|  3  |  交易顺序依赖  |  frontrunning相关攻击   |
|  4  |  时间戳依赖  |  与交易时间相关的攻击  |
|  5  |  拒绝服务  |  通过意外回滚或gaslimit导致的拒绝服务  |
|  6  |  权限管理  |  因逻辑缺陷导致的权限丢失等安全问题  |

&emsp;&emsp;有关上述漏洞的详细介绍及漏洞合约数据集参见[链接](https://swcregistry.io/)。  
&emsp;&emsp;有关该检测工具的更多介绍参见[链接](https://github.com/Jianbo-Gao/EasyFlow)。


### 针对Go链码

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [Basic writing and formatting syntax](https://docs.github.com/en/github/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/my-code-cloud/SafeSmartContract/settings/pages). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://docs.github.com/categories/github-pages-basics/) or [contact support](https://support.github.com/contact) and we’ll help you sort it out.

---
layout: default
---

Text can be **bold**, _italic_, or ~~strikethrough~~.

[Link to another page](./another-page.html).

There should be whitespace between paragraphs.

There should be whitespace between paragraphs. We recommend including a README, or a file with information about your project.

# Header 1

This is a normal paragraph following a header. GitHub is a code hosting platform for version control and collaboration. It lets you and others work together on projects from anywhere.

## Header 2

> This is a blockquote following a header.
>
> When something is important enough, you do it even if the odds are not in your favor.

### Header 3

```js
// Javascript code with syntax highlighting.
var fun = function lang(l) {
  dateformat.i18n = require('./lang/' + l)
  return true;
}
```

```ruby
# Ruby code with syntax highlighting
GitHubPages::Dependencies.gems.each do |gem, version|
  s.add_dependency(gem, "= #{version}")
end
```

#### Header 4

*   This is an unordered list following a header.
*   This is an unordered list following a header.
*   This is an unordered list following a header.

##### Header 5

1.  This is an ordered list following a header.
2.  This is an ordered list following a header.
3.  This is an ordered list following a header.

###### Header 6

| head1        | head two          | three |
|:-------------|:------------------|:------|
| ok           | good swedish fish | nice  |
| out of stock | good and plenty   | nice  |
| ok           | good `oreos`      | hmm   |
| ok           | good `zoute` drop | yumm  |

### There's a horizontal rule below this.

* * *

### Here is an unordered list:

*   Item foo
*   Item bar
*   Item baz
*   Item zip

### And an ordered list:

1.  Item one
1.  Item two
1.  Item three
1.  Item four

### And a nested list:

- level 1 item
  - level 2 item
  - level 2 item
    - level 3 item
    - level 3 item
- level 1 item
  - level 2 item
  - level 2 item
  - level 2 item
- level 1 item
  - level 2 item
  - level 2 item
- level 1 item

### Small image

![Octocat](https://github.githubassets.com/images/icons/emoji/octocat.png)

### Large image

![Branching](https://guides.github.com/activities/hello-world/branching.png)


### Definition lists can be used with HTML syntax.

<dl>
<dt>Name</dt>
<dd>Godzilla</dd>
<dt>Born</dt>
<dd>1952</dd>
<dt>Birthplace</dt>
<dd>Japan</dd>
<dt>Color</dt>
<dd>Green</dd>
</dl>

```
Long, single-line code blocks should not wrap. They should horizontally scroll if they are too long. This line should be long enough to demonstrate this.
```

```
The final element.
```
