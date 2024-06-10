# Tips & tricks

## Hard to style windows

There are windows that disappear on unfocus or after some action, copy & paste the following in the SharedJSContext console and open them again:

```js
g_PopupManager.AddPopupCreatedCallback((e) => {
  setTimeout(() => {
    const popup = e.m_popup;
    const popup_doc = popup.document;
    const new_wnd = window.open(
      "about:blank?browserType=6",
      popup_doc.title,
      `width=${popup.innerWidth},height=${popup.innerHeight}`
    );

    new_wnd.document.write(popup_doc.documentElement.outerHTML);
  }, 1_000);
});
```

This will open the exact same window that will not disappear. The titlebar buttons (and everything else) on created windows will not work, so the system titlebar will be added. To remove it, delete the `?browserType=6` part.

The `1_000` indicates that the window's HTML will be copied to the new one after a second. This may not always work, and so you may have to increase it.

Note that this affects every single window, including notifications, game overlay, etc. You will have to revert this once you're done:

```js
g_PopupManager.m_rgPopupCreatedCallbacks.pop();
```

## Readable class names

The class names got completely obfuscated [one day](https://github.com/SteamDatabase/SteamTracking/commit/a0f82423f4c422f616253d5825fd8bf453367f3a), so you may use [this gist](https://gist.github.com/ricewind012/3e74b297d28d88af3c84dee028f9cc46) to get readable class names. Copy & paste this in the SharedJSContext console and reopen windows you wish to know the actual class names of.

Note that you can only use them to make comments in your theme, but not use it in your code, because they are applied only for the current Steam session. This also slows down window creation and functionality significantly, so you will have to restart Steam in order to revert this.
