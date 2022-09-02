
# 事件-现场属性（common）

通用属性由其它事件的属性引用，不单独作为事件。

## 设备状态信息（DeviceStatus）

| Attribute | Type | Description | Examples | Requirement Level |
| -- | -- | -- | -- | -- |
| device.status.cpu.app_usage | float | 应用对CPU的占用比例 | 0.3 | Required |
| device.status.cpu.sys_usage | float | 系统对CPU的占用比例 | 0.6 | Required |
| device.status.ram.app_usage | int | 应用内存占用，单位:KB | 104857600 | Required |
| device.status.ram.sys_available | int | 系统可用内存，单位:KB | 1073741824 | Required |
| device.status.rom.sys_available | int | 系统可用存储空间，单位:KB | 1099511627776 | Required |
| device.status.net.signal_strength | int | 设备网络信号强度，取值范围[0,100]，100表示信号强度最大，0表示无信号。 | 80 | Required |

## 用户状态信息（UserStatus）

| Attribute | Type | Description | Examples | Requirement Level |
| -- | -- | -- | -- | -- |
| user.status.login | bool | 用户登录状态 | 1 | Conditionally Required |