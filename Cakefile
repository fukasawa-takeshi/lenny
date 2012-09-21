sys = require 'sys'
fs   = require 'fs'
exec = (require 'child_process').exec

#コンパイルするファイル群
files=[
  'app.coffee'
  'routes/index.coffee'
  'routes/user.coffee'
]

#第二引数の関数は実行が終わった後に呼び出されます。
exec "coffee -cj #{files.join ' '}",(err,stdout,stderr)->
    #エラーや出力結果を出して終わる。
    throw err if err
    console.log stdout+stderr