库函数：
simfang.ttf font.c font.h truetype.h truetype.c 
lcddevice.c lcddevice.h bmp_list.c bmp_list.h 
bmp.c bmp.h
主函数功能实现：
mainfunc.c mainfunc.h
主函数：
main.c
编译管理文件：
Makefile
资源文件：
bmp bmptext.txt mtime.txt text.txt showconfig.txt

说明：
板子屏幕为800*480

关于showconfig.txt的配置，每行配置信息对应，依次为：
开机界面图片显示配置
主界面图片显示配置
滚动显示消息配置
时间显示配置
日期显示配置

每行配置参数依次为：
起点横向坐标 起点纵向坐标 宽 高 文字打印横向坐标 文字打印纵向坐标 文字字体大小

对应范围：
[0,800]  [0,480] [0,800] [0,480] [0,宽] [0,高] [自行决定]

前面四个参数决定了lcd上显示区域大小，后面3个参数决定文字在显示区域内打印的位置及打印的大小，可以知道对显示图片而言，后面3个参数无效，给予0即可。