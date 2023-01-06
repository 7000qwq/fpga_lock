# fpga_lock
Designed and implemented a combination lock system in VIVADO with hardware programming on FPGA using Verilog that can enter, change password, LED light alarm and cancel alarm
Added a status indicator for the password lock, can indicate the current number of correct/incorrect password input, can be a running light to show the alarm
Added jitter elimination to keys to stabilize key input

# Time sequence logic
LED display module
Debounce of OK
3-color-LED display
Flow light

# combinatorial logic
Enter password module

LED分频：
Each number will be turn on in order, to make a visual retention
消抖：
After OK become zero or one for a while, change its value
状态机：
There is a variable to save how many input errors, and the color of LED will change with this variable
