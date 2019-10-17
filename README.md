# MyBox

What's in my github? 我的仓库有些什么？仓库列表，仓库项目，仓库介绍

# 目录

<!--       | 是间隔, :是对齐       -->

| 简介 | 详情 | 备注 |
|-|-|-:|
| <a href="#PoporNetRecord">PoporNetRecord</a>                   | <a href="https://github.com/popor/PoporNetRecord">网络监测</a> | |
| <a href="#PoporNetMonitor">PoporNetMonitor</a>                  | <a href="https://github.com/popor/PoporNetMonitor">网络监测系统请求</a> | |
| <a href="#PoporAFN">PoporAFN</a>                                        | <a href="https://github.com/popor/PoporAFN">网络请求</a> | |
| <a href="#PoporAlertBubbleView">PoporAlertBubbleView</a> | <a href="https://github.com/popor/PoporAlertBubbleView">气泡提示框</a> | |
| <a href="#PoporPlaceholderView">PoporPlaceholderView</a> | <a href="https://github.com/popor/PoporPlaceholderView">UITableView 和 UICollectionView 空白页</a> | |
| <a href="#PoporFFmpegCompress">PoporFFmpegCompress</a>    | <a href="https://github.com/popor/PoporFFmpegCompress">视频压缩 OC 仓库</a> | |
| <a href="#PoporFFmpeg">~~PoporFFmpeg~~</a>                   | <a href="https://github.com/popor/PoporFFmpeg">~~视频压缩 静态库 仓库~~</a> | <a href="https://github.com/popor/PoporFFmpegCommand">推荐PoporFFmpegCommand</a> |
| <a href="#PoporFFmpegLib">~~PoporFFmpegLib~~</a>         | <a href="https://github.com/popor/PoporFFmpegLib">~~FFmpeg 静态库~~</a> | <a href="https://github.com/popor/PoporFFmpegCommand">推荐PoporFFmpegCommand</a>|
| <a href="#FFMpegCompress">~~FFMpegCompress~~</a>     | <a href="https://github.com/popor/FFMpegCompress">~~视频压缩(不完整pod)~~</a>|<a href="https://github.com/popor/PoporFFmpegCommand">推荐PoporFFmpegCommand</a>|
| <a href="#PoporFFmpegCommand">PoporFFmpegCommand</a>  | <a href="https://github.com/popor/PoporFFmpegCommand">基于mobile-ffmpeg</a><a href="#note"><sup> 3 </sup></a>||
| <a href="#PoporIDBankCard">PoporIDBankCard</a>               | <a href="https://github.com/popor/PoporIDBankCard">身份证银行卡识别</a><a href="#note"><sup> 1 </sup></a> | |
| <a href="#PoporUI">PoporUI</a>                                               | <a href="https://github.com/popor/PoporUI">基础UI插件</a> | |
| <a href="#PoporFoundation">PoporFoundation</a>                  | <a href="https://github.com/popor/PoporFoundation">基础Foundation插件</a> | |
| <a href="#PoporFMDB">PoporFMDB</a>                                  | <a href="https://github.com/popor/PoporFMDB">FMDB Sqlite 操作</a> | |
| <a href="#PoporQRCodeIos">PoporQRCodeIos</a>                 | <a href="https://github.com/popor/PoporQRCodeIos">生成二维码图片 iOS</a> <a href="#note"><sup> 1 </sup></a>| |
| <a href="#PoporQRCodeMacos">PoporQRCodeMacos</a>     | <a href="https://github.com/popor/PoporQRCodeMacos">生成二维码图片 macOS</a> <a href="#note"><sup> 1 </sup></a>| |
| <a href="#PoporImageBrower">PoporImageBrower</a>           | <a href="https://github.com/popor/PoporImageBrower">图片浏览</a> <a href="#note"><sup> 1 </sup></a>| |
| <a href="#PoporMedia">PoporMedia</a>                                  | <a href="https://github.com/popor/PoporMedia">图片视频采集浏览</a> <a href="#note"><sup> 1 </sup></a>| |
| <a href="#PoporOrientation">PoporOrientation</a>                  | <a href="https://github.com/popor/PoporOrientation">屏幕旋转</a> | |
| <a href="#PoporAVPlayer">PoporAVPlayer</a>                         | <a href="https://github.com/popor/PoporAVPlayer">视频播放</a> | |
| <a href="#PoporAVPlayer">PoporAVPlayer</a>                         | <a href="https://github.com/popor/PoporAVPlayer">视频播放</a> | |
| <a href="#PoporGhost">PoporGhost</a>                                  | <a href="https://github.com/popor/PoporGhost">一键Ghost</a> | |
| <a href="#PoporDatePicker">PoporDatePicker</a>                  | <a href="https://github.com/popor/PoporDatePicker">获取完整日期</a> <a href="#note"><sup> 1 </sup></a>| |

---

# <a name="PoporNetRecord">PoporNetRecord</a>

To run the example project, clone the repo, and run `pod install` from the Example directory first.

思路模仿自LLDebugTool, https://github.com/HDB-Li/LLDebugTool.git, 但是我只不需要监测所有的网络请求,另外其他需求也不一致,所以有了本framework.

<p>
<img src="https://github.com/popor/PoporNetRecord/blob/master/Example/PoporNetRecord/image/root.png" width="30%" height="30%">
<img src="https://github.com/popor/PoporNetRecord/blob/master/Example/PoporNetRecord/image/list.png" width="30%" height="30%">
<img src="https://github.com/popor/PoporNetRecord/blob/master/Example/PoporNetRecord/image/detail.png" width="30%" height="30%">

</p>

```
电脑浏览器访问,假如使用chrome或者QQ浏览器,安装json-handle插件,可以点击[数据返回]进行更好的查看json数据
```

<p>
<img src="https://github.com/popor/PoporNetRecord/blob/master/Example/PoporNetRecord/image/web1.png" width="100%" height="100%">
<img src="https://github.com/popor/PoporNetRecord/blob/master/Example/PoporNetRecord/image/web2.png" width="100%" height="100%">
<img src="https://github.com/popor/PoporNetRecord/blob/master/Example/PoporNetRecord/image/web3.png" width="100%" height="100%">
</p>

---

# <a name="PoporNetMonitor">PoporNetMonitor</a>

```
pod 'PoporNetMonitor'

兼容iOS和macOS系统
依赖 PoporNetRecord
可以监测系统所有的网络请求
```

---

# <a name="PoporAFN">PoporAFN</a>

```
pod 'PoporAFN'

兼容iOS和macOS系统
依赖 AFNetworking 和 PoporNetRecord
简化 AFNetworking 使用，允许继承自定义设置head，包含一个简单的下载函数。
```

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

# <a name="PoporFFmpegCompress">PoporFFmpegCompress</a>

pod 'PoporFFmpeg'

<p>
<img src='https://github.com/popor/PoporFFmpegCompress/blob/master/Example/PoporFFmpegCompress/screen1.png' width="30%" height="30%">

</p>

##### 缺点使用的是CPU而非GPU进行压缩,会消耗较多时间。可以达到微信视频的压缩质量但是达不到快速压缩。

---

# <a name="PoporFFmpeg">PoporFFmpeg</a>

pod 'PoporFFmpeg'

<p>
<img src='https://github.com/popor/PoporFFmpeg/blob/master/Example/PoporFFmpeg/screen1.png' width="30%" height="30%">

</p>

##### 这个仓库只包括FFmpeg 接口仓库, 生成命令接口在demo,若需要oc接口请使用 PoporFFmpegCompress .

---

# <a name="PoporFFmpegLib">PoporFFmpegLib</a>

这个是生成静态包的项目,因为cocoapod不支持c++的import依赖语法.

---

# <a name="FFMpegCompress">FFMpegCompress(不完整pod)</a>


pod 'FFMpegCompress', :git=>'https://github.com/popor/FFMpegCompress.git', :tag => '0.0.26'

##### 即使加上:tag => '0.0.26',也会在执行update的时候触发下载完整代码的情形,所以推荐使用PoporFFmpeg.
##### ~~一定要带上:tag => '0.0.26',因为没有通过pod验证,假如没有增加会在执行更新'pod update --no-repo-update'.消耗大量时间重新下载FFMpegCompress.~~

##### 缺点使用的是CPU而非GPU进行压缩,会消耗较多时间。可以达到微信视频的压缩质量但是达不到快速压缩。

---

# <a name="PoporFFmpegCommand">PoporFFmpegCommand(基于mobile-ffmpeg)</a>
```
pod 'mobile-ffmpeg-full', '3.1'
pod 'PoporFFmpegTool'

#import <mobileffmpeg/MobileFFmpegConfig.h>
#import <mobileffmpeg/MobileFFmpeg.h>

+ (void)executeCommand:(NSString * _Nonnull)ffmpegCommand finish:(void (^ __nullable)(BOOL executeFinish))finish {
    dispatch_async(dispatch_get_global_queue(DISPATCH_QUEUE_PRIORITY_DEFAULT, 0), ^{
        //NSLog(@"FFmpeg process started with arguments\n\'%@\'\n", ffmpegCommand);
        int result = [MobileFFmpeg execute:ffmpegCommand];
        //NSLog(@"FFmpeg process exited with rc %d\n", result);
        dispatch_async(dispatch_get_main_queue(), ^{
            if (result == RETURN_CODE_SUCCESS) {
                if (finish) {
                    finish(YES);
                }
            } else {
                if (finish) {
                    finish(NO);
                }
            }
        });
    });
}

```
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
-   更改UIImage填充色和背景色，保存图片到指定路径，读取绝对路径图片，压缩图片（指定最大容量、根据size压缩）。
UILabel : 根据UIString、UIFont或者NSAttributedString计算size，
-   UILabelInsets，UILabelPhone。
UINavigationController : 根据Class、index移除某个UIViewController。
UIScrollView : 滑动到最底部，包含 UIScrollView 的VC支持侧滑。
UITableView : UITableViewCell 设定分割线inset。
-   侧滑VC的时候，UITableViewCell跟随滑动渐变色。
UITextField : UIInsetsTextField，UITextField最大输入文字，可以使用RAC替换。
UITextView : UIPasteImageTextView，
-   UIPlaceHolderTextView，
-   UITextView (MaxLength)，
-   UITextView (Size)
UIView : UIView (Extension)
UIViewController : UIViewController (AC: iPad弹出UIAlertControl sheet 模式的时候不崩溃，设定默认popPresenter.sourceRect)，
-   设定导航栏按钮，
-   导航栏是否隐藏BOOL，
-   UIViewController (TapEndEdit: 点击空白处关闭键盘，键盘高度变化接口)。
```

---

# <a name="PoporFoundation">PoporFoundation</a>

```
pod 'PoporFoundation'

兼容iOS和macOS系统
KVO : 安全的 NSObject (WMSafeKVO)
NSArray : 安全的NSArray，防止nil、越界等bug；
NSArray (jsonDic) 转 json；
NSMutableArray (chain) 链式函数；
NSAssistant : 根据 runtime 为 NSObject 从 NSDictionary 提取对应 value。
根据 runtime 把 NSObject NSLog 所有 value。
NSData : NSData (dic) 生成 Json NSDictionary。
NSDate : 时间的一些函数。
NSDecimalNumber : 链式函数，安全屏蔽。
NSDictionary : 安全屏蔽，to jsonString。
NSFileManager : 常用函数
NSObject : NSObject (Swizzling)；
-   NSObject (performSelector) 无警告执行Selector;
-   NSObject (assign) 给NSObject设定value
NSString : NSString (email) 判断是否是email；
-   NSString (format) 简化 NSMutableAttributedString；
-   NSString (IDCard) 判断是否是大陆身份证；
-   NSString (MD5)
-   NSString (Size) 计算size；
-   NSString (Tool) 正则操作函数；
NSURL : NSURL (Swizzling) 安全屏蔽
PrefixCore : PrefixBlock，PrefixColor，PrefixFont，PrefixFun，PrefixSize 常用宏
PrefixOs : iOS 和 macOS 兼容宏
```

---

# <a name="PoporFMDB">PoporFMDB</a>

```
pod 'PoporFMDB'

兼容iOS和macOS系统

包括根据 NSObject 自动创建 TABLE，生成 SQL 语句；
自动检查 NSObject 参数变化更新 TABLE，不支持删除、更改属性类型。
简化查询函数
```

---

# <a name="PoporQRCodeIos">PoporQRCodeIos</a>

```
pod 'PoporQRCodeIos'

生成二维码图片
摘自于:
https://github.com/Chris-Pan
http://www.jianshu.com/users/e2f2d779c022/latest_articles
```

---

# <a name="PoporQRCodeMacos">PoporQRCodeMacos</a>

```
pod 'PoporQRCodeMacos'

生成二维码图片
摘自于:  
https://github.com/shibiao/QRCodeGenerated
```

---

# <a name="PoporImageBrower">PoporImageBrower</a>

```
pod 'PoporImageBrower'

查看图片: URL和本地图片方式，下滑图片关闭等特效。
摘自于: 
https://github.com/zhoushaowen/SWPhotoBrower, 除了原作者URL之外,增加了UIImage查看模式.
```

---

# <a name="PoporMedia">PoporMedia</a>

```
pod 'PoporMedia'

依赖:
SKFCamera: 拍摄图片和视频，支持连拍图片。
TZImagePickerController: 读取本地iCloud的图片视频。
PoporImageBrower: 图片浏览
```

---

# <a name="PoporOrientation">PoporOrientation</a>

```
pod 'PoporOrientation'

#import <PoporOrientation/PoporOrientation.h>

1.设置
- (BOOL)application:(UIApplication *)application didFinishLaunchingWithOptions:(NSDictionary *)launchOptions
{
[PoporOrientation swizzlingAppDelegate:self];
return YES;
}

2.AppDelegate中增加
- (UIInterfaceOrientationMask)application:(UIApplication *)application supportedInterfaceOrientationsForWindow:(nullable UIWindow *)window {
// this will be replaced by PoporOrientation within runtime, do not remove!
return UIInterfaceOrientationMaskPortrait;
}

3.可以设置自动旋转，或者优先旋转到某个方向等。
```

---

# <a name="PoporAVPlayer">PoporAVPlayer</a>

```
pod 'PoporAVPlayer'

支持本地和url播放视频。

NSString *videoPath = [[NSBundle mainBundle] pathForResource:@"douyin" ofType:@"mp4"];
NSURL * videoURL    = [NSURL fileURLWithPath:videoPath];

videoURL = [NSURL URLWithString:@"https://yiche-static.oss-cn-hangzhou.aliyuncs.com/anjie/uploads/video/20181009/88b3d738583bb6c6c00c0c5f19fc381a.mp4"];
[self.navigationController pushViewController:[PoporAVPlayerVCRouter vcWithDic:@{@"title":@"升降桌", @"videoURL":videoURL, @"showLockRotateBT":@(YES)}] animated:YES];
```

---

# <a name="PoporGhost">PoporGhost</a>
```
目的: 方便测试数据, 将测试数据转变为dic,通过yyCache保存到磁盘,可以在下一次恢复,适用于大量输入数据的情况.

#import "PoporGhost.h"
#import <ReactiveObjC/ReactiveObjC.h>

- (void)ghostAction {
    // 防止block循环引用
    @weakify(self);
    PoporGhostBlockRestore blockRestore;
    PoporGhostBlockVoid blockDisappear;
    
    // 恢复block
    blockRestore = ^(NSDictionary * restoreDic, NSString * description, NSString * time, NSString * version) {
        @strongify(self);
        self.testEntity = [TestEntity yy_modelWithDictionary:restoreDic];
        
        self.nameTF.text = self.testEntity.name;
        self.addTF.text  = self.testEntity.add;
        
        [self.navigationController popViewControllerAnimated:YES];
    };
    
    // ghost页面关闭block
    blockDisappear = ^(void) { };
    
    self.testEntity.name = self.nameTF.text;
    self.testEntity.add  = self.addTF.text;
    
    // 设置dic
    NSDictionary * dic;
    dic = @{
        @"blockRestore":blockRestore,
        @"blockDisappear":blockDisappear,
        @"title":@"记录", // 下个页面title
        @"saveKey":NSStringFromClass(self.view.class), // yyCache保存到磁盘的key
        @"saveDic":self.testEntity.yy_modelToJSONObject, // 需要保存的dic
    };
    
    [self.navigationController pushViewController:[[PoporGhost alloc] initWithDic:dic]  animated:YES];
}
```

<p>
<img src="https://github.com/popor/PoporGhost/blob/master/Example/Classes/image/screen1.png" width="30%" height="30%">
<img src="https://github.com/popor/PoporGhost/blob/master/Example/Classes/image/screen2.png" width="30%" height="30%">
<img src="https://github.com/popor/PoporGhost/blob/master/Example/Classes/image/screen3.png" width="30%" height="30%">
</p>


# <a name="PoporDatePicker">获取完整日期</a>
```ruby
pod 'PoporDatePicker'
```

该仓库复制于 https://github.com/Zws-China/DatePicker , 由于作者使用了xib, 代码无法直接运行; 移除了部分不需要的函数, 标准命名规则;

<p>
<img src="https://github.com/popor/PoporDatePicker/blob/master/Example/screen/screen1.png" width="30%" height="30%">
<img src="https://github.com/popor/PoporDatePicker/blob/master/Example/screen/screen2.png" width="30%" height="30%">

</p>


# <a name="test">test</a>

---

# <a name="note">注意</a>
1. 借用他人代码整理成cocoapod插件
2. 他人cocoapod插件
3. 依赖他人cocoapod插件

## Author

popor, 908891024@qq.com
