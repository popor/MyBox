<a href='https://github.com/popor/mybox'> MyBox </a>

# 置顶 Simulator 分为2种方法

前提需要开启 SID: 重启Mac, 调出 terminal 执行 csrutil disable
开机后运行 Simulator

# 1.通过 Xcode 调试执行
首先依次点击 Debug > Attach To Process > Simulator
( 参考于:  https://apple.stackexchange.com/questions/219116/any-nice-stable-ways-to-keep-a-window-always-on-top-on-the-mac/245154#answer-368717 )
<p>
<img src="https://github.com/popor/MyBox/blob/master/stayInFront/note1.png" width="60%" height="60%">
</p>

点击暂停程序按钮
<p>
<img src="https://github.com/popor/MyBox/blob/master/stayInFront/note2.png" width="30%" height="30%">
</p>

然后通过 LLDB 命令操作 Simulator 窗口实现置顶，缺点：即使点击了继续程序按钮，仍然不能关闭该xcode调试状态，否则 Simulator 会退出运行。
<p>
<img src="https://github.com/popor/MyBox/blob/master/stayInFront/note3.png" width="50%" height="50%">
</p>

LLDB 命令
```
e NSApplication $app = [NSApplication sharedApplication]
e NSWindow $win = $app.windows[0]

e [$win setLevel: 3]  // NSFloatingWindowLevel=3, 置顶
e [$win setLevel: 0]  // NSNormalWindowLevel=0, 普通 取消置顶

```

# 2.通过 Terminal 执行 LLDB
打开 terminal，直接赋值下面代码到 terminal 直接运行即可，分别为置顶和取消置顶的命令。

```
lldb
process attach --name Simulator
e NSApplication $app = [NSApplication sharedApplication];
e NSWindow $win = $app.windows[0];
e [$win setLevel: 3];
exit
y

```
---

```
lldb
process attach --name Simulator
e NSApplication $app = [NSApplication sharedApplication];
e NSWindow $win = $app.windows[0];
e [$win setLevel: 0];
exit
y

```

```
ps: 升级到 Mac10.15 之后，Simulator 会存在2个以上的进程，这个时候打开管理器，查看真正的是哪个
把 ‘process attach --name Simulator’ 换为 ‘process attach --pid 12694’ 就可以正常使用了.

```
<p>
<img src="https://github.com/popor/MyBox/blob/master/stayInFront/note4.png" width="50%" height="50%">
</p>


# 同样的方法可以适用于其他 APP

## Author

popor, 908891024@qq.com
