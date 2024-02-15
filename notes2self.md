# Newline in TextMate

<https://github.com/microsoft/vscode-textmate/issues/41>

Hi, I'm trying to expand the support for my plugin, graphql-for-vscode, to support gherkin feature files, but I'm stuck while defining the grammer. The begin regexp seems to not do any matching when I specify a newline (\n).

I've spent some time browsing other syntaxes in vscode and textmate, but could only find \n to be used in match regexp sections, but none yet in begin or end sections.

I also tried running npm run inspect on my syntax definition, and see that the tokenizer takes one line at a time. So, it seems like it's not possible to define multi-line begin/end rules? If not, then is there an alternate?