# 主题色设置

得益于 MDUI 框架，MDr 包含了 19 种主色和 16 种强调色。前往 [颜色和主题 - MDUI 文档](https://www.mdui.org/docs/color) 可以阅读更多。

## 主题主色

默认为 `indigo` 。

<div>
<button data-md-color-primary="red">Red</button>
<button data-md-color-primary="pink">Pink</button>
<button data-md-color-primary="purple">Purple</button>
<button data-md-color-primary="deep-purple">Deep Purple</button>
<button data-md-color-primary="indigo">Indigo</button>
<button data-md-color-primary="blue">Blue</button>
<button data-md-color-primary="light-blue">Light Blue</button>
<button data-md-color-primary="cyan">Cyan</button>
<button data-md-color-primary="teal">Teal</button>
<button data-md-color-primary="green">Green</button>
<button data-md-color-primary="light-green">Light Green</button>
<button data-md-color-primary="lime">Lime</button>
<button data-md-color-primary="yellow">Yellow</button>
<button data-md-color-primary="amber">Amber</button>
<button data-md-color-primary="orange">Orange</button>
<button data-md-color-primary="deep-orange">Deep Orange</button>
<button data-md-color-primary="brown">Brown</button>
<button data-md-color-primary="grey">Grey</button>
<button data-md-color-primary="blue-grey">Blue Grey</button>
</div>

<script>
var buttons = document.querySelectorAll("button[data-md-color-primary]");
Array.prototype.forEach.call(buttons, function(button) {
    button.addEventListener("click", function() {
        document.body.dataset.mdColorPrimary = this.dataset.mdColorPrimary;
    })
})
</script>

## 主题强调色

默认为 `pink` 。

<div>
<button data-md-color-accent="red">Red</button>
<button data-md-color-accent="pink">Pink</button>
<button data-md-color-accent="purple">Purple</button>
<button data-md-color-accent="deep-purple">Deep Purple</button>
<button data-md-color-accent="indigo">Indigo</button>
<button data-md-color-accent="blue">Blue</button>
<button data-md-color-accent="light-blue">Light Blue</button>
<button data-md-color-accent="cyan">Cyan</button>
<button data-md-color-accent="teal">Teal</button>
<button data-md-color-accent="green">Green</button>
<button data-md-color-accent="light-green">Light Green</button>
<button data-md-color-accent="lime">Lime</button>
<button data-md-color-accent="yellow">Yellow</button>
<button data-md-color-accent="amber">Amber</button>
<button data-md-color-accent="orange">Orange</button>
<button data-md-color-accent="deep-orange">Deep Orange</button>
</div>

<script>
var buttons = document.querySelectorAll("button[data-md-color-accent]");
Array.prototype.forEach.call(buttons, function(button) {
    button.addEventListener("click", function() {
        document.body.dataset.mdColorAccent = this.dataset.mdColorAccent;
    })
})
</script>

## 主题强调色 ( Dark Mode )

该选项所配置的是 `Dark Mode` 开启时的主题强调色，与 `Dark Mode` 关闭时的主题强调色互不影响互不干扰。

## Chrome 顶栏颜色

即未开启 `Dark Mode` 时的 `meta["theme-color"]` 的值，为十六进制颜色码，默认为 `#ffffff`。