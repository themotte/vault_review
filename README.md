Welcome to the Motte Quality Vault Reviews!

Would you like to help review and edit [vault](https://www.vault.themotte.org/) entries? We've got some work for you to do!

----

Here's the first prototype instructions, let me know if anything is unclear.

* Fork this repo, then clone your fork using Git.
* Go to the Issues page. Leave a comment on a post block saying that you're handling it (so nobody else grabs it.)
* Look over the entries in the numbered post block and edit them as per the instructions near the end.
* Check in your work, push it, and send a [pull request](https://docs.github.com/en/github/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request).
* Repeat as you have time!

----

Post editing instructions:

In general, most of the things in a post shouldn't be edited, with two exceptions.

The first and most important exception is the title. Some of the titles just weren't intended for publication. Look at the title (in &lt;title&gt; tags) and, if necessary, modify it for publication. Titles should be spelled properly, punctuated properly, and capitalized properly as per [title case](https://en.wikipedia.org/wiki/Title_case) ([converter here](https://titlecase.com/), use AP-Style Title Case). They should not have a trailing period or exclamation point and should not be written as clickbait unless there's a really good reason (I'd accept "Ten TERRIFYING things you didn't know about clickbait!", for example). Check out [the Vault's homepage](https://www.vault.themotte.org/) for examples.

The second exception is context quotes. [Some posts](https://www.vault.themotte.org/post/the_internets_effect_on_publishing) just make no sense without an introductory quote to see what they were responding to. On Reddit, people just hit "parent" and go read the context, but that's not an option here. Prepend www.reddit.com to the &lt;link&gt; and go visit it to see what it looks like; if it makes a lot more sense with a parent, you need to add a context quote.

The right way to do this is to create a &lt;context&gt; block before the &lt;body&gt;, then copy all relevant context in there. You can use full HTML in this block; please copy any formatting from your quotes as well (Inspect Element in your favorite web browser makes this easy, just copy and paste!) You can also nest quotes with &lt;blockquote&gt; tags.

If the post includes an existing but insufficient &lt;blockquote&gt;, move it out of the &lt;body&gt; and into a &lt;context&gt; with extra quotes as necessary. This is the only time you should be editing a &lt;body&gt;!

Examples of much of this can be found in the [example_before](https://github.com/themotte/vault_review/tree/master/example_before) and [example_after](https://github.com/themotte/vault_review/tree/master/example_after) directories. Title editing is shown in ymeskhout's post, &lt;context&gt; is added in Amadanb's, ymeskhout's, and ZorbaTHut's posts, with an existing blockquote hoisted from &lt;body&gt; to &lt;context&gt; in ZorbaTHut's example.

If you're not entirely sure what to do with a post, do it anyway. Everything submitted will be reviewed by me; I'd rather have your best guess at the right solution than anything else. If you *really* don't know what to do with it, move it into a folder named REVIEW_ME and I'll handle it.

Finally, don't feel like you have to edit a post! Sometimes they're fine as-is.

Thank you in advance for your help!

----

Did you find a problem in the live site? There's currently no way for people to help me with that directly, but post an issue, with the URL included, and tell me what the problem is; I'll take care of it. Thank you also!