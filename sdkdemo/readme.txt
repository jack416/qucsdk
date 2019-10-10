第一步：插件法的自定义控件使用，务必保证编译器完全一致。
第二步：将对应的quc.dll和libquc.a 或者 quc.lib(MSVC编译器才有)集成到项目中。
第三步：使用到哪个控件，只需要将对应控件的头文件集成到项目中即可。集成方法是将该头文件复制到sdk目录（因为pro文件写的是从sdk目录读取头文件），也可以自己定义目录。
第四步：项目的pro文件加入代码
INCLUDEPATH += $$PWD/sdk

CONFIG(release, debug|release){
LIBS        += -L$$PWD/sdk/ -lquc
} else {
unix {LIBS  += -L$$PWD/sdk/ -lquc}
else {LIBS  += -L$$PWD/sdk/ -lqucd}
}

说明：本sdkdemo下的dll是mingw 64位+Qt5.12.3版本的。可自行替换成自己编译器编译出来的文件。两个文件都要替换，msvc编译器是dll+lib，mingw编译器是dll+a，gcc编译器是so，clang编译器是dylib。务必记得debug就用debug的，release就用release的，不能交叉用，比如debug编译出来的dll放到release中用，是万万不可以的。