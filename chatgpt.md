写出详细过程
此项目fork自https://github.com/electron-vite/electron-vite-vue
需要添加串口通信功能
首页上部下拉列表列出所有连接到电脑的串口，用户选则合适的串口点击连接，开始监控串口发来的数据
接收到数据格式是{'time':25488962, 'CH1':[23,45],'CH2':[23,56]}
将数据保存到sqlite3数据库

1. 安装包
npm install serialport --save

Import the serialport module in the main file (main.js) of our Electron app:

const SerialPort = require('serialport');

Use the SerialPort.list() method to get a list of all available serial ports:

SerialPort.list().then((ports) => {
  console.log(ports);
}).catch((error) => {
  console.error(error);
});


使用plotlyjs在网页中实时显示数据库中的数据，横坐标是当前时间