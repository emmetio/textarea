# [Emmet](http://emmet.io) plugin for &lt;textarea&gt;

*This plugin is automatically compiled from the [Emmet core](https://github.com/emmetio/emmet). If you want to contribute features or fix bugs, please do this in [plugin source](https://github.com/emmetio/emmet/tree/master/plugins/textarea).*

******

To add Emmet support and  basic code editor features (like Tab key handler and formatted linebreak insertion) to your `<textarea>` boxes:

1. Add `<script src="emmet.min.js"></script>` into your page
2. Run this JavaScript code:

```js
emmet.require('textarea').setup({
	pretty_break: true, // enable formatted line breaks (when inserting 
			            // between opening and closing tag) 
	use_tab: true       // expand abbreviations by Tab key
});

```

Additionally, you can add special classes to your `<textarea>` element to control Emmet behavior:

* `emmet-syntax-NAME`: set syntax `NAME` for current `<textarea>`: `html`, `css`, `xml` etc.
* `emmet-profile-NAME`: set one of the [predefined profile](http://docs.emmet.io/customization/syntax-profiles/#predefined-profiles).
* `emmet-use_tab-BOOL`: enable (`yes`) or disable (`no`) Tab expander on current `<textarea>`.
* `emmet-pretty_break-BOOL`: enable (`yes`) or disable (`no`) formatted linebreak insertion on current `<textarea>`.
* `no-emmet`: disable Emmet actions on current `<textarea>`.

## Overriding keybindings

To override default keybindings, simply create global `emmetKeymap` object, the same as [default one](https://github.com/emmetio/emmet/blob/master/plugins/textarea/controller.js#L8) but with your own keybindings.



