## Solution Summary

XSS.

Idea: insert a post with Javascript code. When loaded, the Javascript will load the page that shows you your password, copy it, and share it as a post. The tricky part is that posts are not allowed to use quotes, so you have to get around it by cleverly using `String.fromCharCode()`.

## Solution Details

TODO: get actual JS inserted.

## Problem Statement (Copied from CTF website)

After Karma Trader from Level 4 was hit with massive karma inflation (purportedly due to someone flooding the market with massive quantities of karma), the site had to close its doors. All hope was not lost, however, since the technology was acquired by a real up-and-comer, Streamer. Streamer is the self-proclaimed most steamlined way of sharing updates with your friends. You can access your Streamer instance here: https://level06-2.stripe-ctf.com/user-zmxjwhyoms

The Streamer engineers, realizing that security holes had led to the demise of Karma Trader, have greatly beefed up the security of their application. Which is really too bad, because you've learned that the holder of the password to access Level 7, level07-password-holder, is the first Streamer user.

As well, level07-password-holder is taking a lot of precautions: his or her computer has no network access besides the Streamer server itself, and his or her password is a complicated mess, including quotes and apostrophes and the like.

Fortunately for you, the Streamer engineers have decided to open-source their application so that other people can run their own Streamer instances. You can obtain the source for Streamer at git clone https://level06-2.stripe-ctf.com/user-zmxjwhyoms/level06-code. We've also included the most important files below.
