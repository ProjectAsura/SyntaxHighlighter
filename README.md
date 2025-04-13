# SyntaxHighlighter
Custom brush for SyntaxHighlighter Evolved(<https://github.com/Viper007Bond/syntaxhighlighter>).  
HLSL向けのSyntaxHighlighterが無かったので作ってみました。  

# License
This software is distributed under GNU GENERAL PUBLIC LICENSE v3. For details, see LICENCE file.  
ライセンスはSyntaxHighlighter自体がGPLになっているので，本家に合うようGPLにしています。  

## Integration
組み込み方法は3ステップです。  

### Step.1  
SyntaxHighlighter Evolveのthird-party-brushesフォルダに，shBrushHlsl.jsを置きます。  

### Step.2  
syntaxhighlighter.phpを開いて166行目付近に(Register come popular third-party brushesのコメントがあるブロック)  

~~~~~{.php}
		wp_register_script( 'syntaxhighlighter-brush-hlsl',       plugins_url( 'third-party-brushes/shBrushHlsl.js',              __FILE__ ), array('syntaxhighlighter-core'), '20170108'     );
~~~~~

を追加します。

### Step.3  

syntaxhighlighter.phpを開いて209行目付近(haskellの後ぐらい)に  
~~~~~{.php}
			'hlsl'          => 'hlsl',
~~~~~
を追加します。  

### Step.4

syntaxhighlighter.phpを開いて，268行目付近に（haskellの後ぐらい）  
~~~~~{.php}
			'hlsl'       => __( 'HLSL',                      'syntaxhighlighter' ),
~~~~~
を追加します。  


## How to use ?

後は普通のSyntaxHighlighterを適用するのと同じように  

~~~~~{.html}
[hlsl]
code
[/hlsl]
~~~~~

のように鍵かっこタグで挟めば適用されるはずです。  

