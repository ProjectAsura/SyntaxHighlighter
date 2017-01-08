# SyntaxHighlighter
Custom brush for SyntaxHighlighter Evolved.
HLSL������SyntaxHighlighter�����������̂ō���Ă݂܂����B  

# License
This software is distributed under GNU GENERAL PUBLIC LICENSE v3. For details, see LICENCE file.
���C�Z���X��SyntaxHighlighter���̂�GPL�ɂȂ��Ă���̂ŁC�{�Ƃɍ����悤GPL�ɂ��Ă��܂��B  

## Integration
�g�ݍ��ݕ��@��3�X�e�b�v�ł��B

### Step.1
third-party-brushes�t�H���_�ɁCshBrushHlsl.js��u���܂��B

### Step.2 
syntaxhighlighter.php���J����147�s�ڕt�߂�  

~~~~~{.php}
		wp_register_script( 'syntaxhighlighter-brush-hlsl',       plugins_url( 'third-party-brushes/shBrushHlsl.js',              __FILE__ ), array('syntaxhighlighter-core'), '20170108'     );
~~~~~

��ǉ����܂��B

### Step.3

syntaxhighlighter.php���J����185�s�ڕt�߂�  
~~~~~{.php}
			'hlsl'          => 'hlsl',
			'fx'            => 'hlsl',
~~~~~
��ǉ����܂��B  


