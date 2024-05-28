# Preparation
Enter the API key in `app.py`.

You should be fine if you enable the virtual environment. though you need python3.9　or higher

Prepare a domain associated with the port number on localhost.(ngrok)

Also configure the LINE messaging API.

# Usage
1. Enable the virtual environment.
```
$ . myenv/bin/activate
```
2. Run the following command.
```
$ ngrok http 5001
```
3. Open another terminal and run the following code.
```
$ flask run --port 5001 #(specify the port number that is the same as your environment)
```
This will allow you to see the output of the message sent from LINE through Gemini Pro on LINE.
###### The current version does not support images.
###### だいぶ雑に書きましたが詳しくは[Qiita](https://qiita.com/ryo09020/items/6d4f175e8428c6a91eb3)をご覧ください

# 機能
LINEのチャットにてGeminiとおしゃべりができるよ〜
けどngrokはローカルマシンをサーバーとして扱うので常にはできないよ〜今後AWSのlambdaで常にアクセスできるようにする。
