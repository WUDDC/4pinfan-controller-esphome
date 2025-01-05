# 4pinfan-controller-esphome
4pin PWM fan controller and Battery voltage monitoring ，esphome esp8266 esp32
The comments in the file are in simplified Chinese. Please translate them into English if necessary. The comments are already written in great detail.
# 4pin pwm风扇控制＋电池电压采集，esphome
风扇可以单独控制也可以总控，单独控制时转速百分比不会同步到总控滑块，总控滑块调整会同步到单个风扇转速百分比上。
总控默认10为单位步进，最小值设置为50，最大值设置为100，可自行修改
输出引脚的pwm频率设置可以自行修改，大部分风扇都不需要修改！
电压测量使用的是分压电阻的形式进行的测量，请与电池负极使用共地，GND如果不与电池连接测量会不准。
##以下是说明：
#fan_speed ：
    #restore_value: yes #是否保存上次离线转速，默认关闭，如果开启请点击风扇进去看设备实际转速，"风扇同步控制"滑块不会同步当前转速百分比。
    #initial_value: '100' #默认100满转速，可自行设置。建议50，因为有的风扇可能是反的，100是停转，请自行确认
#fan1、fan2
#如果你使用了单风扇调整功能，您单风扇的值不会同步到"风扇同步控制"滑块。
请自行更新配置文件内的api key、mqtt设置、ota设置的内容，当然也可以使用我文件里的，bin文件对应就是我的配置，使用“ https://web.esphome.io ”进行刷入就行
