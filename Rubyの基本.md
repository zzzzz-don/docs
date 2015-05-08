# Rubyの基本

## Arrayクラス

### 配列の生成
```
irb(main):001:0> array = []
=> []
```
```
irb(main):002:0> array = Array.new
=> []
```
```
irb(main):003:0> array = [1, "two", ['one', 2], :four]
=> [1, "two", ["one", 2], :four]
```

### 配列へのアクセス
```
irb(main):004:0> a = [1, 2, 3, 4, 5, 6]
=> [1, 2, 3, 4, 5, 6]
irb(main):005:0> a[0]
=> 1
irb(main):006:0> a[-1]
=> 6
```

### 要素の追加
```
irb(main):008:0> array.push 5
=> [1, "two", ["one", 2], :four, 5]
irb(main):009:0> array << "six"
=> [1, "two", ["one", 2], :four, 5, "six"]
```

### 要素の数
```
irb(main):010:0> array.length
=> 6
irb(main):011:0> array.size
=> 6
```
