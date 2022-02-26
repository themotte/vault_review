Welcome to the Motte Quality Vault Reviews!

Would you like to help review and edit [vault](https://www.vault.themotte.org/) entries? We've got some work for you to do!

# Post editing instructions

* Fork this repo, then clone your fork using Git.
* Go to the [Issues](https://github.com/themotte/vault_review/issues) page. Add an issue with the block number saying that you're handling it (so nobody else grabs it.)
* Look over the entries in the numbered post block and edit them as per the instructions near the end.
* Check in your work, push it, and send a [pull request](https://docs.github.com/en/github/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request).
* Repeat as you have time!

In general, most of the things in a post shouldn't be edited, but there's a few things that need to be dealt with.

## Titles

Some of the titles currently provided just weren't intended for publication. Look at the title (in &lt;title&gt; tags) and, if necessary, modify it for publication. Titles should be spelled properly, punctuated properly, and capitalized properly as per [title case](https://en.wikipedia.org/wiki/Title_case) ([converter here](https://titlecase.com/), use AP-Style Title Case). They should not have a trailing period or exclamation point and should not be written as clickbait unless there's a really good reason (I'd accept "Ten TERRIFYING things you didn't know about clickbait!", for example). Check out [the Vault's homepage](https://www.vault.themotte.org/) for examples.

## Context

[Some posts](https://www.vault.themotte.org/post/the_internets_effect_on_publishing) just make no sense without an introductory quote to see what they were responding to. On Reddit, people just hit "parent" and go read the context, but that's not an option here. Prepend www.reddit.com to the &lt;link&gt; and go visit it to see what it looks like; if it makes a lot more sense with a parent, you need to add a context quote.

The right way to do this is to create a &lt;context&gt; block before the &lt;body&gt;, then copy all relevant context in there. You can use full HTML in this block; please copy any formatting from your quotes as well (Inspect Element in your favorite web browser makes this easy, just copy and paste!) You can also nest quotes with &lt;blockquote&gt; tags.

If the post includes an existing but insufficient &lt;blockquote&gt;, move it out of the &lt;body&gt; and into a &lt;context&gt; with extra quotes as necessary.

Examples of much of this can be found in the [example_before](https://github.com/themotte/vault_review/tree/master/example_before) and [example_after](https://github.com/themotte/vault_review/tree/master/example_after) directories. Title editing is shown in ymeskhout's post, &lt;context&gt; is added in Amadanb's, ymeskhout's, and ZorbaTHut's posts, with an existing blockquote hoisted from &lt;body&gt; to &lt;context&gt; in ZorbaTHut's example.

If the &lt;body&gt; has a lot of busted or weird HTML tags, feel free to strip them out; we want normal formatting, not whatever markup Reddit decides to attach to everything.

## Category

Every post needs a &lt;category&gt; tag, with one to three categories wrapped in &lt;li&gt; &lt;/li&gt; pairs (again, check out the examples). The categories are:

*Coteries*: Groups of people self-organized by a shared label; sometimes political, sometimes historical, sometimes based on faith or things adjacent to it. If we must talk about groups in terms of individuals, this is where it goes. "Liberals" and "Conservatives", "Red" and "Blue", any time people decide to love or hate based solely on self-identification.

*Culture*: The beliefs, faiths, identity, and tendencies of people as a group, as described by trends rather than self-labeling. When we divide people based on action and statistics.

*Personal*: People interacting directly and individually, not en masse, not based on label. Romance, management, and the workplace, in no particular order.

*Knowledge*: The process of becoming better at things. Intelligence and education, science and engineering, rationality and logic.

*Economics*: Supply and demand. Game theory. People or organizations making decisions based on the hand of the market, regardless of what form that hand takes. Money, often, but not always.

*Civilization*: What keeps us together? What does it all mean? History, law, morality, and philosophy. 

*Moloch*: Everything getting worse, despite the intentions of everyone. Records of inexorable erosion. A shrine for the things we, as a species, must fight, or be overwhelmed by.

*Media*: Writing, movies, music, and art. Fiction and non-fiction. Goblins and journalism.

*Flux*: Progress, positive and negative, perhaps intentional, perhaps accidental. The change of things over time. 

These categories are intentionally vague and kind of ill-defined. Look at the Motte front page for examples, but trust your gut here; if it feels right, it's probably right.

## Deletion

If the post was deleted by the user while leaving their account active, make a `deleted` subdirectory in the block subdirectory, and move it in there. If the user deleted their account but not the post, or deleted their account and *all* posts, then (1) do the normal post edit things listed above, and (2) make an `anonymized` directory in the block subdirectory and move it in there. (The codebase doesn't support anonymous entries yet, so I'll just shove them off in a corner of the database until I've got that implemented.)

## Notes

Is there a note you want attached to the post permanently, in case someone later comes along to edit it? Add a <notes> block and write whatever you want in there.

## Golden Rule

If you're not entirely sure what to do with a post, do it anyway. Everything submitted will be reviewed by me; I'd rather have your best guess at the right solution than anything else. If you *really* don't know what to do with it, move it into a folder named REVIEW_ME and I'll handle it.

Finally, with the exception of categories, don't feel like you have to edit a post! Sometimes they're fine as-is. (But they really do need categories added.)

Thank you in advance for your help!

# Live Site Editing

Did you find a problem in a post already on the live site? There's currently no way for people to help me with that directly, but post an issue, with the URL included, and tell me what the problem is; I'll take care of it. Thank you also!