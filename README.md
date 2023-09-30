# elect_archive

```
cargo install trunk
cargo install cargo-edit
rustup target add wasm32-unknown-unknown

mkdir elect_archive
cd elect_archive
cargo init
cargo add dioxus
cargo add dioxus-web
```

[index.html]
```
<html>
  <head>
    <meta content="text/html;charset=utf-8" http-equiv="Content-Type" name="viewport" content="width=device-width, initial-scale=1.0" charset="UTF-8">
  </head>
  <body>
    <div id="main"> </div>
  </body>
</html>
``
[main.rs]
```
#![allow(non_snake_case)]
use dioxus::prelude::*;

fn main() {
    dioxus_web::launch(App);
}

fn App(cx: Scope) -> Element {
    cx.render(rsx! {
        div {
            "Hello, world!"
        }
    })
}
```

```
trunk serve
http://localhost:8080
```
