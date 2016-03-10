# What does `doctype` do?

The **`doctype`** declaration or **Document Type Definition** is a statement that is a required preamble for html pages.

It is not a tag, but is needed for legacy reasons.

> When performing HTML validation testing on a web page it tells the HTML (HyperText Markup Language) validator which version of (X)HTML standard the web page coding is supposed to comply with. When you validate your web page the HTML validator checks the coding against the applicable standard then reports which portions of the coding do not pass HTML validation (are not compliant).

When you don't add `doctype` to an HTML page things can break. HTML validation and proper CSS implementation requires the `doctype` declaration.

The `doctype` is just one of many Document Type Definitions. You can find a full list [here](https://www.w3.org/QA/2002/04/valid-dtd-list.html).