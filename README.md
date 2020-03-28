# Edit Chrome Textarea
[![Melpa](https://melpa.org/packages/edit-chrome-textarea-badge.svg)](https://melpa.org/#/edit-chrome-textarea)

This is an Emacs package for editing Chrome textarea through [Chrome DevTools
Protocol](https://chromedevtools.github.io/devtools-protocol).

## Usage

To use this package, you need to enable Chrome DevTools Protocol by launching
Chrome with `--remote-debugging-port=9222`, if you are on macOS, you can use

    $ open -a Google\ Chrome --args --remote-debugging-port=9222

1. Select the textarea you want to edit in Chrome
2. Switch to Emacs, type `M-x edit-chrome-textarea` to open a buffer pre-filled
   with the textarea's content
3. Hit `C-c C-c` to send text in current buffer back to Chrome or `C-c C-k` to
   discard


## Alternatives

- the edit-server package, https://github.com/stsquad/emacs_chrome
- the atomic-chrome package, https://github.com/alpha22jp/atomic-chrome

### Comparison with atomic-chrome

Pros:

- Don't need to install a browser extension

Cons:

- Users need to enable Chrome DevTools Protocol
- Edit-chrome-textarea can't sync between Chrome and Emacs on-the-fly (it's
  possible with Chrome DevTools Protocol but beyond my skills)
- Edit-chrome-textarea can't understand editable div such as CodeMirror used by
  GitHub (it's also possible but beyond my skills)

## Requires

- Emacs 25.1
- the websocket package, https://github.com/ahyatt/emacs-websocket
