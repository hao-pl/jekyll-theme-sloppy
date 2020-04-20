---
layout: post
title:  "Jekyll site 元素测试"
mathjax: true
date:   2020-03-22 8:11:13
categories: Jekyll
tags: ['Markdown','Jekyll']
excerpt: Jekyll中的markdown元素测试
---

* content
{:toc}
## Code Blocks

```ruby
def print_hi(name)
  puts "Hi, #{name}"
end
print_hi('Tom')
#=> prints 'Hi, Tom' to STDOUT.
```
```c
#include "stdio.h"
int main(void)
{
    printf("heloooooooooooooo/n");
}
```

## Mathjax

在Markdown中，有两种输入公式的方法：一是行内公式（inline），用一对美元符包裹。二是整行公式（displayed），用一对紧挨的两个美元符号$$包裹。

这是一个行内公式$E=m c^{2}$，写法是：`$E=mc^2$`。

这是一个整行公式：
$$
\sum_{i=0}^n i^2 = \frac{(n^2+n)(2n+1)}{6}
$$

## 下标

H<sub>2</sub>O<sub>2</sub>
{:.text-center}

```html
H<sub>2</sub>O<sub>2</sub>
```

## Block quote

> 聪明才智之士，勇武有力之人，极大多数是积极进取的。道德标准把他们划分为两类：努力目标是为大多数人谋福利的，是好人；只着眼于自己的权力名位、物质欲望，而损害旁人的，是坏人。好人或坏人的大小，以其嘉惠或损害的人数和程度而定。政治上大多数时期中是坏人当权，于是不断有人想取而代之；有人想进行改革；另有一种人对改革不存希望，也不想和当权派同流合污，他们的抉择是退出斗争漩涡，独善其身。所以一向有当权派、造反派、改革派，以及隐士。中国的传统观念，是鼓励人“学而优则仕”，学孔子那样“知其不可而为之”，但对隐士也有极高的评价，认为他们清高。隐士对社会并无积极贡献，然而他们的行为和争权夺利之徒截然不同，提供了另一种范例。中国人在道德上对人要求很宽，只消不是损害旁人，就算是好人了。《论语》记载了许多隐者，晨门、楚狂接舆、长沮、桀溺、荷丈人、伯夷、叔齐、虞仲、夷逸、朱张、柳下惠、少连等等，孔子对他们都很尊敬，虽然，并不同意他们的作风。

## Notice & Label

```markdown
Success Text.
{:.success}

Info Text.
{:.info}

Warning Text.
{:.warning}

Error Text.
{:.error}

`success`{:.success}`info`{:.info}`warning`{:.warning}`error`{:.error}
```

Success Text.
{:.success}

Info Text.
{:.info}

Warning Text.
{:.warning}

Error Text.
{:.error}

`success`{:.success}`info`{:.info}`warning`{:.warning}`error`{:.error}

## Video
```html

获得ID的方式：点击分享中间的aid后边的数字即为所求。如

<iframe src="//player.bilibili.com/player.html?aid=96854770&bvid=BV1T7411Z7gx&cid=165347352&page=1" scrolling="no" border="0" frameborder="no" framespacing="0" allowfullscreen="true"> </iframe>

### 多页面选择

<div>{%- include extensions/bilibili.html id='12050822' page="2" -%}</div>
不填默认为1

### YouTube

<div>{/%- include extensions/youtube.html id='0W8uPF5aIYo' -/%}</div>

### TED

<div>{/%- include extensions/ted.html id='emily_esfahani_smith_there_s_more_to_life_than_being_happy' -/%}</div>

### bilibili 

<div>{/%- include extensions/bilibili.html id='18428155' -/%}</div>

```

### YouTube

<div>{%- include extensions/youtube.html id='0W8uPF5aIYo' -%}</div>

### TED

<div>{%- include extensions/ted.html id='emily_esfahani_smith_there_s_more_to_life_than_being_happy' -%}</div>

### bilibili 

<div>{%- include extensions/bilibili.html id='18428155' -%}</div>

## Emoji

:soccer::sleeping::cheese::laughing::blush::smiley::relaxed::smirk::heart_eyes::kissing_heart::kissing_closed_eyes::flushed::satisfied::grin::wink::grinning::kissing::kissing_smiling_eyes::stuck_out_tongue::sleeping::worried::frowning::anguished::open_mouth::grimacing::confused::hushed::expressionless::unamused::sweat_smile::disappointed_relieved::weary::pensive::disappointed::confounded::fearful::cold_sweat::persevere::cry::sob::joy::astonished::scream::angry::rage::triumph::sleepy::yum::mask:

## Gif

![](/assets/post-img/earth.gif){: .img-default}

##  Player

<div>{%- include extensions/video.html id='assets/videos/10-sleep-habits.mp4' -%}</div>
<div>{%- include extensions/audio.html id='assets/audios/hktk.mp3' -%}</div>

```markdown
<div>{/%- include extensions/video.html id='assets/videos/10-sleep-habits.mp4' -%}</div>
<div>{/%- include extensions/audio.html id='assets/audios/hktk.mp3' -%}</div>
记得用<div> </div> 包裹
```

## Buttons
[Click me](http://www.google.com){: .btn} [Click me](http://www.google.com){: .btn-g} [Click me](http://www.google.com){: .btn-y}  [Click me](http://www.google.com){: .btn-r} [Click me](http://www.google.com){: .btn-b}

```markdown
[Click me](http://www.google.com){: .btn} [Click me](http://www.google.com){: .btn-g} [Click me](http://www.google.com){: .btn-y}  [Click me](http://www.google.com){: .btn-r} 
[Click me](http://www.google.com){: .btn-b}
```