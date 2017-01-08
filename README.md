# SyntaxHighlighter
Custom brush for SyntaxHighlighter Evolved.
HLSL向けのSyntaxHighlighterが無かったので作ってみました。  

# License
This software is distributed under GNU GENERAL PUBLIC LICENSE v3. For details, see LICENCE file.
ライセンスはSyntaxHighlighter自体がGPLになっているので，本家に合うようGPLにしています。  

## Integration
組み込み方法は3ステップです。

### Step.1
third-party-brushesフォルダに，shBrushHlsl.jsを置きます。

### Step.2 
syntaxhighlighter.phpを開いて147行目付近に  

~~~~~{.php}
		wp_register_script( 'syntaxhighlighter-brush-hlsl',       plugins_url( 'third-party-brushes/shBrushHlsl.js',              __FILE__ ), array('syntaxhighlighter-core'), '20170108'     );
~~~~~

を追加します。

### Step.3

syntaxhighlighter.phpを開いて185行目付近に  
~~~~~{.php}
			'hlsl'          => 'hlsl',
			'fx'            => 'hlsl',
~~~~~
を追加します。  


