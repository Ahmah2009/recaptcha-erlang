I created this driver for use with yaws, but there is no specific reason it can't be used with any other erlang webserver, or even your own. It's just an erlang module!

Instructions:
  1. Download
  1. Unzip
  1. Replace the fake private key with your private key
  1. Compile (erlc recaptcha.erl)
  1. Call `recaptcha_check_answer(RemoteIp, Challenge, Response) -> {Line1, Line2}`
    * `RemoteIp = string()`
    * `Challenge = string()`
    * `Response = string()`
    * `Line1 = string()`
    * `Line2 = string()`

See http://recaptcha.net/apidocs/captcha/ for contents of Line1 and Line 2 under "Verifying the reCAPTCHA Solution" :: "Response"