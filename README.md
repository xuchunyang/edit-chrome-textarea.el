# Edit Chrome Textarea

This is an Emacs package for editing Chrome textarea through [Chrome DevTools
Protocol](https://chromedevtools.github.io/devtools-protocol).

## Usage

1. Select the textarea you want to edit in Chrome
2. Switch to Emacs, type `M-x edit-chrome-textarea` to open a buffer pre-filled
   with the textarea's content
3. Hit `C-c C-c` to send text in current buffer back to Chrome or `C-c C-k` to
   discard

## Requires

- Emacs 25.1
- the websocket package, https://github.com/ahyatt/emacs-websocket

## Alternatives

- the edit-server package, https://github.com/stsquad/emacs_chrome
- the atomic-chrome package, https://github.com/alpha22jp/atomic-chrome
