# lunar [![License](https://img.shields.io/badge/license-MIT-4EB1BA.svg?style=flat-square)](https://github.com/6tail/lunar-php/blob/master/LICENSE)

lunar是一款无第三方依赖的公历(阳历)和农历(阴历、老黄历)工具，支持星座、儒略日、干支、生肖、节气、节日、彭祖百忌、每日宜忌、吉神宜趋、凶煞宜忌、吉神(喜神/福神/财神/阳贵神/阴贵神)方位、胎神方位、冲煞、纳音、星宿、八字、五行、十神、建除十二值星、青龙名堂等十二神、黄道黑道日及吉凶等。

> 基于php5.3开发，由于数值计算精度问题导致节气交接时刻的计算有少许偏差。

[English](https://github.com/6tail/lunar-php/blob/master/README_EN.md)

## 示例

    <?php
    include 'lunar.php';
     
    use com\nlf\calendar\Lunar;
     
    $lunar = Lunar::fromYmd(1986,4,21);
    echo $lunar->toFullString()."\n";
    echo $lunar->getSolar()->toFullString()."\n";

输出结果：

    1986-05-29 00:00:00 星期四 双子座
    壹玖捌陆年肆月廿一 丙寅(虎)年 癸巳(蛇)月 癸酉(鸡)日 子(鼠)时 纳音[炉中火 长流水 剑锋金 桑柘木] 星期四 北方玄武 星宿[斗木獬](吉) 彭祖百忌[癸不词讼理弱敌强 酉不会客醉坐颠狂] 喜神方位[巽](东南) 阳贵神方位[巽](东南) 阴贵神方位[震](正东) 福神方位[兑](正西) 财神方位[离](正南) 冲[(丁卯)兔] 煞[东]

## 文档

请移步至 [http://6tail.cn/calendar/api.html](http://6tail.cn/calendar/api.html "http://6tail.cn/calendar/api.html")

## 联系

<a target="_blank" href="https://jq.qq.com/?_wv=1027&k=5F9Pbf0"><img border="0" src="http://pub.idqqimg.com/wpa/images/group.png" alt="lunar" title="lunar"></a>
