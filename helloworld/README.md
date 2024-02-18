![](../assets/images/wallpaper.jpeg)

## configure golang environment in vscode

go version go1.21.4 windows/amd64

### install golang relevant tools

```
go env -w GOPROXY=https://goproxy.cn,direct
```

Windows平台按下 `Ctrl+Shift+P`，Mac平台按 `Command+Shift+P`，这个时候VS Code界面会弹出一个输入框，输入 `go: install` 记得重启VS Code。

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

### configure user snippets

配置自定义代码片段（snippet）

setting -> user snippet -> edit json

### fix golang problem [unprocessed]

> gopls was not able to find modules in your workspace.
> When outside of GOPATH, gopls needs to know which modules you are working on.
> You can fix this by opening your workspace to a folder inside a Go module, or
> by using a go.work file to specify multiple modules.
> See the documentation for more information on setting up your workspace:
> https://github.com/golang/tools/blob/master/gopls/doc/workspace.md


```
2024	2025	2026	2027	2028	2029	2030	2031	2032	2033	2034
25		26		27		28		29		30		31		32		33		34		35
8		16		16		16		20		20		20		20		25		25		25
8		10+0	1		1		0+15	30		30		30		35		35		35
0		-5		-15		-15		-5		10		10		10		10		10		10
-40										60
+20
```
