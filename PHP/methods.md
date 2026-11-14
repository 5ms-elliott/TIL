# filter_var() 
  指定された値に対してフィルターを適用する  
    ```filter_var ( mixed $variable [, int $filter = FILTER_DEFAULT [, mixed $options ]] ) ```  
    
  主な使用例： 
  - メールアドレス、URL、IPアドレスの検証
  - 整数値の検証と範囲チェック 
  - 特殊文字のサニタイズ 

# array_key_exists() 
  キーが配列内に存在するか確認する。  
  キーが存在する場合はtrue、存在しない場合にfalseを返す。  
  ```array_key_exists(string|int|float|bool|resource|null $key, array $array)```  
  
  isset()との違い:  
      array_key_exists関数は配列の値がNULLでもtrueを返しますが、isset関数はfalseを返す。 

# flush()
  出力バッファに蓄積されたデータをクライアントに送信するよう、PHPに指示する。 
  ```void flush(void)``` 

  ユースケース：  
    長時間実行処理の進捗表示  
    ファイルダウンロードの進捗表示  
    CLIのプログレスバー   

# array_chunk()
  配列を指定したサイズで分割する関数。大きな配列を複数の小さな部分配列に分割することが可能。  
  ```array_chunk(配列, 分割するサイズ, キーの保持)``` 

 使用例：  
 ```$color = array("red", "blue", "yellow", "green", "purple");  
 $result = array_chunk($color, 2);  
 print_r($result);

 Array
 (  
  [0] => Array 
  (  
     [0] => red  
     [1] => blue 
  )  
  [1] => Array  
  (  
     [0] => yellow  
     [1] => green  
  )  
  [2] => Array  
  (  
     [0] => purple 
  )  
)
```

# 引数の参照渡し（リファレンス渡し） 
定義する関数の引数の前に「＆」を付加する。 
```
<?php 
function set_bono(&$var) { 
  $var = 'bonobono'; 
} 

$name = 'hogehoge'; 
echo $name . '<br>'; /* hogehoge 表示 */ 

set_bono($name); 
echo $name . '<br>'; /* bonobono 表示 */ 
?>
```
$name と $var は同じメモリアドレスを指し示す（エイリアス、別名）ので、 呼び出し元の変数$nameも'bonobono'に書き換わる。 

# array_column() 
多次元配列の中から特定のカラムの値を簡単に抽出する。  
```array_column(array $array, int|string|null $column_key, int|string|null $index_key = null): array ```

### 使用例 
```
$books = [ 
  ['book_id' => 1, 'book_name' => 'PHP入門'], 
  ['book_id' => 2, 'book_name' => 'JavaScript基礎'], 
  ['book_id' => 3, 'book_name' => 'Python応用'] 
]; 

$result = array_column($books, 'book_name'); 
print_r($result); 

array 
( 
  [0] => PHP入門 
  [1] => JavaScript基礎 
  [2] => Python応用 
)
```

# is_scaler()
指定した式がスカラー値として評価されるかを調べます。   
スカラー値：　int, float, string, bool のいずれか  
```is_scalar(mixed $value): bool``` 
