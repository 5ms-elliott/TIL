## Closure クラス 
無名関数を表すために使うクラス。  
無名関数は、Closure 型のオブジェクトを生成します。 このクラスにはメソッドが用意され、 生成した無名関数をさらにコントロールできるようになっています。  
 <table>
    <tr>
      <td>Closure::__construct</td>
      <td>インスタンス作成を無効化したコンストラクタ</td>
    </tr>
    <tr>
      <td>Closure::bind</td>
      <td>バインドされたオブジェクトとクラスのスコープでクロージャを複製する</td>
    </tr>
    <tr>
      <td>Closure::bindTo</td>
      <td>新しくバインドしたオブジェクトとクラスのスコープで、クロージャを複製する</td>
    </tr>
    <tr>
      <td>Closure::call</td>
      <td>クロージャを束縛して呼び出す</td>
    </tr>
    <tr>
      <td>Closure::fromCallable</td>
      <td>callable をクロージャに変換する</td>
    </tr>
    <tr>
      <td>Closure::getCurrent</td>
      <td>現在実行中のクロージャを返す</td>
    </tr>
 </table>

## クラス名::class 
::classとは、クラスの完全修飾名を文字列として取得するための記述で、PHP5.5から導入されたものです。  
PHP8.0以降は、オブジェクト（インスタンス）に対しても ::class を使って、そのクラスの完全修飾名を取得することができます。  
例えば、名前空間「App\Service」の中の「TestClass」の完全修飾名は「App\Service\TestClass」です。  
このため、名前空間「App\Service」の中で「echo TestClass::class」を実行すると「App\Service\TestClass」が返ってきます。 
