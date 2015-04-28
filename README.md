練習問題3.1
スクリプトで最後の行を最初に持ってきたスクリプトに変更し実行する。

repeat_lyrics()
def print_lyrics():
  print "I'm a lumberjack, and I'm okay. "
  print "I sleep all night and I work all day."
def repeat_lyrics():
  print_lyrics()
  print_lyrics()

実行結果
Traceback (most recent call last):
  File "ex3-1.py", line 1, in <module>
    print_lyrics()
NameError: name 'print_lyrics' is not defined

練習問題3.2
同様に関数定義のrepeat_lyricsをprint_lyricsの前で行いスクリプトする

def repeat_lyrics():
  print_lyrics()
  print_lyrics()
def print_lyrics():
  print "I'm a lumberjack, and I'm okay. "
  print "I sleep all night and I work all day."
repeat_lyrics()

実行結果
I'm a lumberjack, and I'm okay.
I sleep all night and I work all day.
I'm a lumberjack, and I'm okay.
I sleep all night and I work all day.

練習問題3.3
pythonは文字列の長さを返す組み込み関数len（len('allen')は5を返す。）
文字列の表示で、文字列の最後の文字が70桁にくるような
right_justify関数を作成

>>> def rigth_justify(allen):
...      print "%70s" % allen
...
>>> rigth_justify('allen')
                                                                 allen
