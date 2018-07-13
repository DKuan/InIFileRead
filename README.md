# InIFileRead
INI文件读取C++库（修改版）
在INI配置文件中，原先的数据读取只能做到取出对应整数或者浮点数，但是对于数组的取出有点麻烦，因此修改增加了Array的操作。
示例：需要设为如下格式
[student]
ages=(0012,0023,0034,) 根据逗号识别，往前搜索4位，圆括号与方括号只是为了区分不同数组方便
Get_Array(string root, string key, float *Data, int num) 最后一个num是设置要读取的数据个数
