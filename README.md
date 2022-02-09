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
