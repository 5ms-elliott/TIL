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
