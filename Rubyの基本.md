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

## Hashクラス

### ハッシュの生成
```
irb(main):012:0> hash = {red: 'eagle', blue: 'shark', yellow: 'panther'}
=> {:red=>"eagle", :blue=>"shark", :yellow=>"panther"}
```
```
irb(main):013:0> sunbalkan = Hash.new
=> {}
irb(main):014:0> sunbalkan[:red] = 'eagle'
=> "eagle"
irb(main):015:0> sunbalkan[:blue] = 'shark'
=> "shark"
irb(main):016:0> sunbalkan[:yellow] = 'panther'
=> "panther"
irb(main):017:0> sunbalkan
=> {:red=>"eagle", :blue=>"shark", :yellow=>"panther"}
```

### バリューへのアクセス
```
irb(main):018:0> hash[:red]
=> "eagle"
```

## イテレータ

(参考) http://qiita.com/kidach1/items/651b5b5580be40ad047e

### Arrayクラスをイテレータで回す
```
irb(main):027:0> array.each do |i|
irb(main):028:1*   puts i
irb(main):029:1> end
1
two
one
2
four
5
six
=> [1, "two", ["one", 2], :four, 5, "six"]
```

### Hashクラスをイテレータで回す(キー、バリュー)
```
irb(main):023:0> hash.each do |key, val|
irb(main):024:1*   puts "key=#{key} value=#{val}"
irb(main):025:1> end
key=red value=eagle
key=blue value=shark
key=yellow value=panther
=> {:red=>"eagle", :blue=>"shark", :yellow=>"panther"}
```

### Hashクラスをイテレータで回す(キーのみ)
```
irb(main):047:0> hash.each_key do |key|
irb(main):048:1*   puts key
irb(main):049:1> end
red
blue
yellow
=> {:red=>"eagle", :blue=>"shark", :yellow=>"panther"}
```

### Hashクラスをイテレータで回す(バリューのみ)
```
irb(main):050:0> hash.each_value do |val|
irb(main):051:1*   puts val
irb(main):052:1> end
eagle
shark
panther
=> {:red=>"eagle", :blue=>"shark", :yellow=>"panther"}
```


