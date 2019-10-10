#### 项目介绍
Qt编写的自定义控件插件的sdk集合，包括了各个操作系统的动态库文件以及控件的头文件和sdk使用demo。

#### 版本说明
1. sdk目录下分old目录和V日期的目录，其中old为早期版本。
2. 其他文件夹为对应日期的版本，而且同时提供了debug和release的动态库。
3. 头文件请使用对应文件夹下的头文件，因为控件一直在升级完善。
4. 强烈推荐使用最新版，目前共163个控件。

#### 目录说明
1. include目录为控件对应的头文件
2. sdk目录为各个Qt版本对应的动态库文件，
3. sdk目录还包含所有控件的效果演示可执行文件和安卓apk文件
4. sdkdemo目录为演示如何调用动态库文件
5. snap目录为各个控件的运行效果图,一直更新

#### 特别说明
**动态库和对应的头文件会一直更新完善修复BUG，由于作者精力有限，不保证所有的插件都是最新的，只保证qt_5_7_0_mingw530_32这个版本永远是最新的正确的，为什么选择这个版本，因为5.7.0是最后一个支持XP的版本。谢谢信任和理解。**

#### 功能特点
 1. 超过160个精美控件，涵盖了各种仪表盘、进度条、进度球、指南针、曲线图、标尺、温度计、导航条、导航栏，flatui、高亮按钮、滑动选择器、农历等。远超qwt集成的控件数量。
 2. 每个类都可以独立成一个单独的控件，零耦合，每个控件一个头文件和一个实现文件，不依赖其他文件，方便单个控件以源码形式集成到项目中，较少代码量。qwt的控件类环环相扣，高度耦合，想要使用其中一个控件，必须包含所有的代码。
 3. 全部纯Qt编写，QWidget+QPainter绘制，支持Qt4.6到Qt5.13的任何Qt版本，支持mingw、msvc、gcc等编译器，支持任意操作系统比如windows+linux+mac+嵌入式linux等，不乱码，可直接集成到Qt  Creator中，和自带的控件一样使用，大部分效果只要设置几个属性即可，极为方便。
 4. 每个控件都有一个对应的单独的包含该控件源码的DEMO，方便参考使用。同时还提供一个所有控件使用的集成的DEMO。
 5. 每个控件的源代码都有详细中文注释，都按照统一设计规范编写，方便学习自定义控件的编写。
 6. 每个控件默认配色和demo对应的配色都非常精美。
 7. 超过130个可见控件，6个不可见控件。
 8. 部分控件提供多种样式风格选择，多种指示器样式选择。
 9. 所有控件自适应窗体拉伸变化。
 10. 集成自定义控件属性设计器，支持拖曳设计，所见即所得，支持导入导出xml格式。
 11. 自带activex控件demo，所有控件可以直接运行在ie浏览器中。
 12. 集成fontawesome图形字体+阿里巴巴iconfont收藏的几百个图形字体，享受图形字体带来的乐趣。
 13. 所有控件最后生成一个dll动态库文件，可以直接集成到qtcreator中拖曳设计使用。
 14. 目前已经有qml版本，后期会考虑出pyqt版本，如果用户需求量很大的话。

![avatar](https://gitee.com/feiyangqingyun/QUCSDK/raw/master/snap/000.gif)
![avatar](https://gitee.com/feiyangqingyun/QUCSDK/raw/master/snap/00.gif)
![avatar](https://gitee.com/feiyangqingyun/QUCSDK/raw/master/snap/0.gif)
![avatar](https://gitee.com/feiyangqingyun/QUCSDK/raw/master/snap/0.png)
![avatar](https://gitee.com/feiyangqingyun/QUCSDK/raw/master/snap/1_qtcreator_msvc2017.png)
![avatar](https://gitee.com/feiyangqingyun/QUCSDK/raw/master/snap/customring.gif)
![avatar](https://gitee.com/feiyangqingyun/QUCSDK/raw/master/snap/gaugecar.gif)
![avatar](https://gitee.com/feiyangqingyun/QUCSDK/raw/master/snap/gaugecolor.gif)
![avatar](https://gitee.com/feiyangqingyun/QUCSDK/raw/master/snap/gaugemini.gif)
![avatar](https://gitee.com/feiyangqingyun/QUCSDK/raw/master/snap/gaugepanel.gif)
![avatar](https://gitee.com/feiyangqingyun/QUCSDK/raw/master/snap/gaugepercent.gif)
![avatar](https://gitee.com/feiyangqingyun/QUCSDK/raw/master/snap/gaugespeed.gif)
![avatar](https://gitee.com/feiyangqingyun/QUCSDK/raw/master/snap/progresspercent.gif)
![avatar](https://gitee.com/feiyangqingyun/QUCSDK/raw/master/snap/telwidget.gif)
![avatar](https://gitee.com/feiyangqingyun/QUCSDK/raw/master/snap/wavebar.gif)
![avatar](https://gitee.com/feiyangqingyun/QUCSDK/raw/master/snap/switchbutton.gif)