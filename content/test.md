---
title: Bootstrap elements
---



## Command prompt

Use the `command` shortcode to generate a block with a default bash command prompt.

<!-- markdownlint-disable MD037 -->
{{< example lang="hugo" >}}
{{</* command */>}}
export MY_VAR=123
{{</* /command */>}}
{{< /example >}}
<!-- markdownlint-enable MD037 -->

Specify `user` and `host` to add the user context to the prompt. In addition, use `(out)` to specify an output line and use `\` to denote a line continuation.

<!-- markdownlint-disable MD037 -->
{{< example lang="hugo" >}}
{{</* command user="user" host="localhost" */>}}
export MY_VAR=123
echo "hello"
(out)hello
echo one \
two \
three
(out)one two three
echo "goodbye"
(out)goodbye
{{</* /command */>}}
{{< /example >}}
<!-- markdownlint-enable MD037 -->

