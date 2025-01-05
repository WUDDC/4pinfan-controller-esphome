# 4pinfan-controller-esphome
4pin PWM fan controller and Battery voltage monitoring ，esphome esp8266 esp32
##以下是说明：
#fan_speed ：
    #restore_value: yes #是否保存上次离线转速，默认关闭，如果开启请点击风扇进去看设备实际转速，"风扇同步控制"滑块不会同步当前转速百分比。
    #initial_value: '100' #默认100满转速，可自行设置。建议50，因为有的风扇可能是反的，100是停转，请自行确认
#fan1、fan2
#如果你使用了单风扇调整功能，您单风扇的值不会同步到"风扇同步控制"滑块。
