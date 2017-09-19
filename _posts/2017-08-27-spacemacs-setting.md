# Spacemacsのインストールと設定

## spacemacsのダウンロード
https://github.com/syl20bnr/spacemacs#default-installation

git clone https://github.com/syl20bnr/spacemacs ~/.emacs.d
emacs --insecure

--insecureをつけないと，初回のパッケージダウンロードに失敗して，
エラーが発生するので注意．

## spacemacsの設定
spacemacsでは，.emacs.d/inits.elは特にいじらずに，
.spacemacsで有効にする設定を書く．

### fullscreen設定
dotspacemacs-fullscreen-at-startup t
### layer設定
spacemacsでは各拡張設定はレイヤという単位でまとまっている．
ロードするレイヤを指定する．

dotspacemacs-configuration-layers
'(
;; ----------------------------------------------------------------
;; Example of useful layers you may want to use right away.
;; Uncomment some layer names and press <SPC f e R> (Vim style) or
;; <M-m f e R> (Emacs style) to install them.
;; ----------------------------------------------------------------
helm
auto-completion
better-defaults
emacs-lisp
git
markdown
org
(shell :variables
shell-default-height 30
shell-default-position 'bottom)
spell-checking
syntax-checking
version-control
ruby
ruby-on-rails
python
javascript
html
ansible
yaml

)


### skk等の追加パッケージのインストール
dotspacemacs-additional-packages '(
ddskk
migemo
key-chord
viewer
init-loader
)


### 

