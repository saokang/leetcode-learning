## configure golang environment

go version go1.21.4 windows/amd64

```
go env -w GOPROXY=https://goproxy.cn,direct
```

Windows平台按下`Ctrl+Shift+P`，Mac平台按`Command+Shift+P`，这个时候VS Code界面会弹出一个输入框，输入`go: install` 记得重启VS Code。

出现以下信息即为成功！

```
Tools environment: GOPATH=D:\Environments\gopath
Installing 7 tools at D:\Environments\gopath\bin
  gopls
  gotests
  gomodifytags
  impl
  goplay
  dlv
  staticcheck

Installing golang.org/x/tools/gopls@latest (D:\Environments\gopath\bin\gopls.exe) SUCCEEDED
Installing github.com/cweill/gotests/gotests@v1.6.0 (D:\Environments\gopath\bin\gotests.exe) SUCCEEDED
Installing github.com/fatih/gomodifytags@v1.16.0 (D:\Environments\gopath\bin\gomodifytags.exe) SUCCEEDED
Installing github.com/josharian/impl@v1.1.0 (D:\Environments\gopath\bin\impl.exe) SUCCEEDED
Installing github.com/haya14busa/goplay/cmd/goplay@v1.0.0 (D:\Environments\gopath\bin\goplay.exe) SUCCEEDED
Installing github.com/go-delve/delve/cmd/dlv@latest (D:\Environments\gopath\bin\dlv.exe) SUCCEEDED
Installing honnef.co/go/tools/cmd/staticcheck@latest (D:\Environments\gopath\bin\staticcheck.exe) SUCCEEDED

All tools successfully installed. You are ready to Go. :)
```
