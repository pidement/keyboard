# keyboard
```

(defcfg
  ;; For Linux

  ;; For Windows
  input  (low-level-hook)
  output (send-event-sink)

  ;; For MacOS
  ;; input  (iokit-name "my-keyboard-product-string")
  ;; output (kext)

  ;; Comment this is you want unhandled events not to be emitted
  fallthrough true

  ;; Set this to false to disable any command-execution in KMonad
  allow-cmd true
)

(defsrc
  grv  1    2    3    4    5    6    7    8    9    0    -    =    bspc
  tab  q    w    e    r    t    y    u    i    o    p    [    ]    \
  caps a    s    d    f    g    h    j    k    l    ;    '    ret
  lsft z    x    c    v    b    n    m    ,    .    /    rsft
  lctl lmet lalt           spc            ralt rmet cmp  rctl
)

(deflayer test
  grv  &    7    5    3    1    9    0    2    4    6    8    #    bspc
  tab  ;    <    >    p    y    f    g    c    r    l    /    @    \
  caps a    o    e    u    i    d    h    t    n    s    -    ret
  lsft '    q    j    k    x    b    m    w    v    z    rsft
  lctl lmet lalt           spc            ralt rmet cmp  rctl
)

```
