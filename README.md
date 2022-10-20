# Vosk test

- マイク入力をVoskで日本語文字起こしして、文字起こしした文字列をGoogle Apps Scriptで作成した翻訳APIを通して英語テキストを取得し、pyttsx3で音声出力する。
- Node.jsでやろうとしたら、Windows環境では難易度が高かったので、Pythonを使用。
- [VOSK Models](https://alphacephei.com/vosk/models)からJapaneseのモデルをダウンロードし、カレントディレクトリ直下に`model`ディレクトリとして展開する。
- 環境変数`GAS_URL`にGoogle Apps Scriptで発行されたウェブアプリURL（https://～/exec）を設定する。

参考サイト
- [vosk-api/test_microphone.py at master · alphacep/vosk-api](https://github.com/alphacep/vosk-api/blob/master/python/example/test_microphone.py)
- [3 分で作る無料の翻訳 API with Google Apps Script - Qiita](https://qiita.com/tanabee/items/c79c5c28ba0537112922)
- [nateshmbhat/pyttsx3: Offline Text To Speech synthesis for python](https://github.com/nateshmbhat/pyttsx3)

