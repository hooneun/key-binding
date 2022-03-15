# key-binding

## iterm
- 자동완성: `shift + cmd + ;`
- 최근 디렉토리 히스토리: `Cmd-Opt-/`

## Finder(MAC)
- 폴더 이동: `command + shift + g`

## nvim airline key binding
- 버퍼 새로 열기: `nmap <leader>T :enew<cr>`
- 다음 버퍼로 이동: `nmap <leader>l :bnext<CR>`
- 이전 버퍼로 이동: `nmap <leader>h :bprevious<CR>`
- 현재 버퍼를 닫고 이전 버퍼로 이동 탭 닫기 단축키를 대체한다. `nmap <leader>bq :bp <BAR> bd #<CR>`
- 모든 버퍼와 각 버퍼 상태 출력: `nmap <leader>bl :ls<CR>`

```
" Code navigation shortcuts
nnoremap <silent> <c-]> <cmd>lua vim.lsp.buf.definition()<CR>
nnoremap <silent> K     <cmd>lua vim.lsp.buf.hover()<CR>
nnoremap <silent> gD    <cmd>lua vim.lsp.buf.implementation()<CR>
nnoremap <silent> <c-k> <cmd>lua vim.lsp.buf.signature_help()<CR>
nnoremap <silent> 1gD   <cmd>lua vim.lsp.buf.type_definition()<CR>
nnoremap <silent> gr    <cmd>lua vim.lsp.buf.references()<CR>
nnoremap <silent> g0    <cmd>lua vim.lsp.buf.document_symbol()<CR>
nnoremap <silent> gW    <cmd>lua vim.lsp.buf.workspace_symbol()<CR>
nnoremap <silent> gd    <cmd>lua vim.lsp.buf.definition()<CR>

nnoremap <silent> ga    <cmd>lua vim.lsp.buf.code_action()<CR>

nnoremap <silent> g[ <cmd>lua vim.diagnostic.goto_prev()<CR>
nnoremap <silent> g] <cmd>lua vim.diagnostic.goto_next()<CR>
```

## phpstorm
- Tinker Plugin Open: `ctrl + Shift + T`

## xcode
- File Search: `⌘ + ⇧ + O`

## Golang Snippets
### General
| Prefix  | Content |
| :------- | ------- |
| `vv`   | initialize variable `varName := value`|
| `ier`   | if error `if err != nil { myStatements }` |
| `ifok`   | if ok `if value,ok := myFunc; ok { myStatements } `|
| `fr`   | for range `for _, v := range values { myStatements }`|
| `frr`   | for range channel `for v := range channel { myStatements }`|
| `def`   | case default `default:` |
| `cl`   | close `close(closable)` |
| `fms`   | fmt Sprinf `fmt.Sprintf("%+v", args)` |


### Types
| Prefix  | Content |
| :------- | ------- |
| `st`   | struct type <pre>type structName struct {<br/>}</pre>|
| `sf`   | struct field `fieldName string`|
| `stt`   | struct tag `` `json:"jsonFieldName"` ``|
| `ne`   | struct constructor method <pre>func NewFoo() *Foo{<br/>  return &Foo {<br/>  }<br/>}</pre>|
| `inte`   | Interface type <pre>type interfaceName interface {<br/>}|


### Collection manipulation
| Prefix  | Content |
| :------- | ------- |
| `sr`   | remove one element from slice `slice = append(slice[:index], slice[index+1:]...)` |
| `ap`   | append element to slice `slice = append(slice, element)` |
| `del`   | delete map element by key `delete(map, key)`|




### Return values
| Prefix  | Content |
| :------- | ------- |
| `rn`   | Return Nil `return nil`|
| `rne`   | Return Nil and err `return nil, err`|
| `re`   | Return err `return err`|


### Logging
| Prefix  | Content |
| :------- | ------- |
| `lo`   | log variable `log.Printf("%+v\n", varName)` |
| `le`   | log error `log.Printf("%+v\n", err)` |


### Error Handling
| Prefix  | Content |
| :------- | ------- |
| `es`   | errors with stack `errors.WithStack(err)`|
| `em`   | error with message `errors.WithMessage(err, message)`|
| `emf`   | error with messagef `errors.WithMessagef(err, format, args)`|
| `is`   | errors Is `if errors.Is(err, MyError) { myStatements }`|
| `as`   | errors As <pre>var e ErrorType<br/>errors<span>.</span>As(err, &e) {<br/>  myStatements<br/>}</pre> |


### Concurrency
| Prefix  | Content |
| :------- | ------- |
| `gofunc`   | anonymous go function `go func() { myStatements }` |
| `defunc`   | anonymous defer function `defer func { myStatements }`|
| `lock`   | sync.Mutex Lock and defer Unlock <pre>mu.Lock()<br/>defer mu.Unlock()</pre>|
| `nb` | non-blocking channel send <pre>select {<br/>case msg &lt;- msgChan:<br/>default:<br/>}</pre>|


[code]: https://code.visualstudio.com/
[coffee]: https://buy.stripe.com/9AQ9DA6qq3Afbrq7ss

