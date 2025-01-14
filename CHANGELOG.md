## 1.0.0

### Enhancements

* Tokenization encoding/decoding is now fully customizable
* Signed GlobalID tokenization supported (#22)
* Turbo is now properly supported (#23, #33 - thanks @iainbeeston and @til!)
* More thorough integration testing using a dummy Rails app
* Added a Rails engine to solve loading issues and tidy up file structuring
* `Passwordless::SessionsController` now uses gem source instead of needing to be generated from a template
* `MagicLinksController` no longer requires a weird `routes.rb` entry to work
* `MagicLinksController` now uses gem source instead of needing to be generated from a template
* `magic_link_(path|url)` view helpers are now implemented for all resources (cleans up mailer view template)
* Tokenizer encoding now supports `:expires_at` option (#19, #21 - thanks @JoeyLeadJig and @bvsatyaram!)
* Users will be redirected after magic link is sent (customized using `after_magic_link_sent_path_for`)

### Bugfixes

* Requiring `Devise::Passwordless::Mailer` should no longer cause errors
