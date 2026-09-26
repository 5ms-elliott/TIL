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
