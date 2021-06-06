遅くなってごめんなさい。
確認した結果、resource/message/index.blade.phpのところで記述ミスが見つかりました。修正すれば画像が登録できると思います。

resource/message/index.blade.php : 18行目

誤：
```
<form method="post" action="{{ url('/messages') }}" entype="multipart/form-data">
```

正：
```
<form method="post" action="{{ url('/messages') }}" enctype="multipart/form-data">
```


