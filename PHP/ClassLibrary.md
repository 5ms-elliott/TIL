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
