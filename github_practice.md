# リポジトリ作成方法(github)
1. githubにログインしてリポジトリを開いて、新しいリポジトリを作る
2. sshをコピーして
3. git bashで作りたいフォルダの場所で `git clone <sshキー>`
4. lsで確認して、githubで作ったファイル(sshキー)にcdで移動

# Vite + Reactインストール
1. `npm create vite@latest`(選択肢の最後らへんはNo)
2. cdで1.で作ったフォルダに移動
3. `code .`でVScodeで開く
4. 開いたらターミナルで`npm install`する(node_modulesがなければ毎回する(node_modulesはgithubには上げない！))
5. `npm run dev`で立ち上げ、残しておく(コマンド打つときは別のターミナルを開く)。`npm run dev`をしたらURLが出てくるので、そのURLをコピペして新しいウィンドウで開くと実際の画面動作などが確認できる 


# クリーンアップ
1. srcフォルダのassetsフォルダとindex.cssを削除
2. publicフォルダのfavicon.svg以外削除
3. https://monotein.com/blog/react-vite-how-to-use これ通りにする

# gitにあげる
1. `git status`で何がcommitされていて何がされていないかを確認できる
2. `git add .`ですべてのファイルをcommitの候補に挙げられる
　ファイルごとにしたい場合は`git add <ファイル名>`
　.gitignoreに書いたファイルは`git add .`しても追加されない
3.  `git status`でaddされているか確認
4. `git commit -m "<コメント>"`でコミットできる
5. `git status`でコミットされているか確認
6. `git push origin main`でorigin(リポジトリ(github上の情報を保存しているところ))にmainブラントをpushしているということ 


