# memo.md
実装中のメモ

# レシピ用のテーブルを作りました
変数名は`recipe_table`で, Pythonの辞書型で格納しています.

名前をつけた理由はテーブルだと思うからです.(意味が間違ってたらすみません)

グローバル変数なので各関数から読み出すことができます.この段階ではオブジェクト指向で実装するというよりも,命令形で実装しています.

# idの振り分けルール
idはファイルの読み込み時に最初のレシピに0をふりそれ以降,+1ずつ加算しています.

# 引数にidを取る
sys.argv[1]に引数が指定されたときに特定のidのみを出力する.

問題がいっぱい.

IDの範囲外を指定してもなぜか違うレシピ名が出てくるので直さなきゃダメ
