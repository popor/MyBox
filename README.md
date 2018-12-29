# MyBox
What's in my github? 我的仓库有些什么？仓库列表，仓库项目，仓库介绍

# 目录
<!-- | 是间隔, :是对齐-->

简介|详情
--|--
<a href="#PoporNetRecord">PoporNetRecord</a>|<a href="https://github.com/popor/PoporNetRecord">网络监测</a>
<a href="#PoporAlertBubbleView">PoporAlertBubbleView</a>|<a href="https://github.com/popor/PoporAlertBubbleView">气泡提示框</a>
<a href="#PoporPlaceholderView">PoporPlaceholderView</a>|<a href="https://github.com/popor/PoporPlaceholderView">UITableView 和 UICollectionView 空白页</a>
<a href="#FFMpegCompress">FFMpegCompress</a>|<a href="https://github.com/popor/FFMpegCompress">视频压缩</a>
<a href="#PoporIDBankCard">PoporIDBankCard</a>|<a href="https://github.com/popor/PoporIDBankCard">身份证银行卡识别<sup>1</sup></a>
<a href="#PoporUI">PoporUI</a>|<a href="https://github.com/popor/PoporUI">基础UI插件</a>
<a href="#PoporFoundation">PoporFoundation</a>|<a href="https://github.com/popor/PoporFoundation">基础Foundation插件</a>

---
# <a name="PoporNetRecord">PoporNetRecord</a>

To run the example project, clone the repo, and run `pod install` from the Example directory first.

思路模仿自LLDebugTool,https://github.com/HDB-Li/LLDebugTool.git,但是我只不需要监测所有的网络请求,另外其他需求也不一致,所以有了本framework.

<p>
<img src="https://github.com/popor/PoporNetRecord/blob/master/Example/PoporNetRecord/image/list.png" width="30%" height="30%">
<img src="https://github.com/popor/PoporNetRecord/blob/master/Example/PoporNetRecord/image/detail.png" width="30%" height="30%">
<img src="https://github.com/popor/PoporNetRecord/blob/master/Example/PoporNetRecord/image/web.png" width="30%" height="30%">
<img src="https://github.com/popor/PoporNetRecord/blob/master/Example/PoporNetRecord/image/set.png" width="30%" height="30%">

</p>

```
电脑浏览器访问,假如使用chrome或者QQ浏览器,安装json-handle插件,可以点击[数据返回]进行更好的查看json数据
```
<p>
<img src="https://github.com/popor/PoporNetRecord/blob/master/Example/PoporNetRecord/image/web1.png" width="100%" height="100%">

</p>

<p>
<img src="https://github.com/popor/PoporNetRecord/blob/master/Example/PoporNetRecord/image/web2.png" width="100%" height="100%">

</p>

---
# <a name='PoporAlertBubbleView'>PoporAlertBubbleView</a>
```
pod 'PoporAlertBubbleView'
类似iPhone 的 UIMenuController,将自定义view以气泡包围的方式展示出来,假如设置的方向不正确则自动使用其他方向.
lableInnerGap更改为customeViewInnerGap,版本迭代产生的命名错误.
```
<p>
<img src="https://github.com/popor/PoporAlertBubbleView/blob/master/Example/image/screen0.png" width="40%" height="40%">
<img src="https://github.com/popor/PoporAlertBubbleView/blob/master/Example/image/screen1.png" width="40%" height="40%">

</p>

---
# <a name="PoporPlaceholderView">PoporPlaceholderView</a>
```
pod 'PoporPlaceholderView'

前提: UITableView和UICollectionView的刷新使用MFRefresh,假如数据为空则显示可以显示默认空白页.
假如需要替换PoporPlaceholderView, 继承PoporPlaceholderView一个即可.
```
<p>
<img src="https://github.com/popor/PoporPlaceholderView/blob/master/Example/PoporPlaceholderView/image/screen1.png" width="40%" height="40%">
</p>


---
# <a name="FFMpegCompress">FFMpegCompress</a>

pod 'FFMpegCompress', :git=>'https://github.com/popor/FFMpegCompress.git', :tag => '0.0.26'

##### 一定要带上:tag => '0.0.26',因为没有通过pod验证,假如没有增加会在执行更新'pod update --no-repo-update'.消耗大量时间重新下载FFMpegCompress.

##### 缺点使用的是CPU而非GPU进行压缩,会消耗较多时间。可以达到微信视频的压缩质量但是达不到快速压缩。

---
# <a name="PoporIDBankCard">PoporIDBankCard</a>

---
# <a name="PoporUI">PoporUI</a>
```
pod 'PoporUI'

兼容iOS和macOS系统
BlockView : iOS8以前的UIAlertView、UIActionSheet采用block模式
IToast : 整理了IToast，import IToastKeyboard.h 使用AlertToastTitle(title)，弹出键盘弹出的时候IToast弹出高度自动上移。
ProgressView : 使用了 https://github.com/gin0606插件。
Response : 根据UIResponder传递事件。
Tool : 包含磁盘空间、设备使用权限、保存图片、APP版本号等信息。
UIButton : 主要是UIButtonLayoutCustom，通过block方式自定义UIButton图片文字frame。
UIDeviceScreen : 获取是否是iPhoneX设备接口。
UIImage : 根据UIColor、NSString、UIFont、UIImage、UIView生成图片，渐变色图片，
          更改UIImage填充色和背景色，保存图片到指定路径，读取绝对路径图片，压缩图片（指定最大容量、根据size压缩）。
UILabel : 根据UIString、UIFont或者NSAttributedString计算size，
          UILabelInsets，UILabelPhone。
UINavigationController : 根据Class、index移除某个UIViewController。
UIScrollView : 滑动到最底部，包含 UIScrollView 的VC支持侧滑。
UITableView : UITableViewCell 设定分割线inset。
UITextField : UIInsetsTextField，UITextField最大输入文字，可以使用RAC替换。
UITextView : UIPasteImageTextView，
             UIPlaceHolderTextView，
             UITextView (MaxLength)，
             UITextView (Size)
UIView : UIView (Extension)
UIViewController : UIViewController (AC: iPad弹出UIAlertControl sheet 模式的时候不崩溃，设定默认popPresenter.sourceRect)，
                   设定导航栏按钮，
                   导航栏是否隐藏BOOL，
                   UIViewController (TapEndEdit: 点击空白处关闭键盘，键盘高度变化接口)。

```

---
# <a name="PoporFoundation">PoporFoundation</a>

```
pod 'PoporFoundation'

兼容iOS和macOS系统
KVO : 安全的 NSObject (WMSafeKVO)
NSArray : 安全的NSArray，防止nil、越界等bug；
          NSArray (jsonDic) 转json；
          NSMutableArray (chain) 链式函数；
NSAssistant : 根据 runtime 为 NSObject 从 NSDictionary 提取对应 value。
              根据 runtime 把 NSObject NSLog 所有 value。
NSData : NSData (dic) 生成 Json NSDictionary。
NSDate : 时间的一些函数。
NSDecimalNumber : 链式函数，安全屏蔽。
NSDictionary : 安全屏蔽，to jsonString。
NSFileManager : 常用函数
NSObject : NSObject (Swizzling)；
           NSObject (performSelector) 无警告执行Selector;
           NSObject (assign) 给NSObject设定value
NSString : NSString (email) 判断是否是email；
           NSString (format) 简化 NSMutableAttributedString；
           NSString (IDCard) 判断是否是大陆身份证；
           NSString (MD5)
           NSString (Size) 计算size；
           NSString (Tool) 正则操作函数；
NSURL : NSURL (Swizzling) 安全屏蔽
PrefixCore : PrefixBlock，PrefixColor，PrefixFont，PrefixFun，PrefixSize 常用宏
PrefixOs : iOS 和 macOS 兼容宏

```

---
# <a name="test">test</a>
---
1. 借用他人代码整理成cocoapod插件

## Author

wangkq, 908891024@qq.com

## License

PoporNetRecord is available under the MIT license. See the LICENSE file for more info.
