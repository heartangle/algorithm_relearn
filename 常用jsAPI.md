# 字符串转小写

toLowerCase

# 字符串转大写

toUpperCase

# 数组常用方法

- pop() 删除数组最后一个元素并返回该元素

# 字符串常用方法

- 截取

```
s.substring(start, end)
// 如果end 超过了字符串长度, 返回空串


slice() 从一个字符串中提取字符串并返回新字符串。在一个字符串中的改变不会影响另一个字符串。也就是说，slice 不会修改原字符串（只会返回一个包含了原字符串中部分字符的新字符串）。

slice() 提取的新字符串包括beginIndex但不包括 endIndex。下面有两个例子。
```

- 字符串补全

```js
padStart; // 从开始位置补全
padEnd; // 从结束位置开始补全

padStart(length, ch); // length 要填充到的长度, 填充字符
```

# Number 常用 api

- floor: 向下取整
- ceil: 向上取整
- round: 给定数字的值四舍五入到最接近的整数。

> 如果参数的小数部分大于 0.5，则舍入到相邻的绝对值更大的整数。 如果参数的小数部分小于 0.5，则舍入到相邻的绝对值更小的整数。如果参数的小数部分恰好等于 0.5，则舍入到相邻的在正无穷（+∞）方向上的整数

# map 的常用操作

```js
const contacts = new Map();
contacts.set("Jessie", { phone: "213-555-1234", address: "123 N 1st Ave" });
contacts.has("Jessie"); // true
contacts.get("Hilary"); // undefined
contacts.set("Hilary", { phone: "617-555-4321", address: "321 S 2nd St" });
contacts.get("Jessie"); // {phone: "213-555-1234", address: "123 N 1st Ave"}
contacts.delete("Raymond"); // false
contacts.delete("Jessie"); // true
console.log(contacts.size); // 1
```

# 编码转换

> 在 JavaScript 中：大写字母 A-Z 对应的 ASCII 码值是 65-90，小写字母 a-z 对应的 ASCII 码值是 97-122，首先我们需要获取用户输入的字符(假设用户每次只能输入一个字符)，然后将输入的字符转换为对应的 ASCII 值，再将转换的 ASCII 值通过 if-else-if 条件语句进行判断，ASCII 的值在 65-90 这个范围内，则是大写的 A-Z；ASCII 的值在 97-122 这个范围内，则是小写的 a-z;ASCII 码的值在 45-57 这个范围内，则是数字 0-9；其他的值则为其他字符。

> str.charCodeAt()：将字符串 str 转换为 ASCII 码
> charCodeAt() 方法可返回指定位置的字符的 Unicode 编码

> String.fromCharCode(strCode):将 ASCII 码转成对应的字符串
> fromCharCode() 可接受一个指定的 Unicode 值，然后返回一个字符串。
