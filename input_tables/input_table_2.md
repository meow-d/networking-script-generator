| name           | type   | in_port | in_device | out_device | out_port | hosts | block_size | subnet_mask     | network_address | broadcast_address | first_usable_address | second_usable_address |
| -------------- | ------ | ------- | --------- | ---------- | -------- | ----- | ---------- | --------------- | --------------- | ----------------- | -------------------- | --------------------- |
| switch5        | switch |         |           | routerGHI  | Fa0/0    | 50    | 2^6 = 64   | 255.255.255.192 | 192.168.70.0    | 192.168.70.63     | 192.168.70.1         | 192.168.70.62         |
| switch6        | switch |         |           | routerGHI  | Fa6/0    | 40    | 2^6 = 64   | 255.255.255.192 | 192.168.70.64   | 192.168.70.127    | 192.168.70.65        | 192.168.70.126        |
| switch0        | switch |         |           | routerABC  | Fa0/0    | 25    | 2^5 = 32   | 255.255.255.224 | 192.168.70.128  | 192.168.70.159    | 192.168.70.129       | 192.168.70.158        |
| switch3        | switch |         |           | routerDEF  | Fa1/0    | 20    | 2^5 = 32   | 255.255.255.224 | 192.168.70.160  | 192.168.70.191    | 192.168.70.161       | 192.168.70.191        |
| switch4        | switch |         |           | routerGHI  | Fa1/0    | 13    | 2^4 = 16   | 255.255.255.240 | 192.168.70.192  | 192.168.70.207    | 192.168.70.193       | 192.168.70.206        |
| switch1        | switch |         |           | routerABC  | Fa1/0    | 10    | 2^4 = 16   | 255.255.255.240 | 192.168.70.208  | 192.168.70.223    | 192.168.70.209       | 192.168.70.222        |
| switch2        | switch |         |           | routerDEF  | Fa0/0    | 5     | 2^3 = 8    | 255.255.255.248 | 192.168.70.224  | 192.168.70.231    | 192.168.70.225       | 192.168.70.230        |
| routersABC-DEF | router | Se2/0   | routerABC | routerDEF  | Se2/0    | 2     | 2^2 = 4    | 255.255.255.252 | 192.168.70.232  | 192.168.70.235    | 192.168.70.233       | 192.168.70.234        |
| routersDEF-GHI | router | Se3/0   | routerDEF | routerGHI  | Se2/0    | 2     | 2^2 = 4    | 255.255.255.252 | 192.168.70.236  | 192.168.70.239    | 192.168.70.237       | 192.168.70.238        |