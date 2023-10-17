# Typeset.css
A relational style sheet for better web typography

## Inspiration

In [_Flexible Typesetting_](https://abookapart.com/products/flexible-typesetting) by Tim Brown, he outlines a simple, straightforward process for achieving great typography on the web. His description of the four core elements of typesetting — typeface, size, measure, and line height — and how to approach them in a particular sequence gave me a better appreciation for how to set browser-based type. Good web typography doesn't happen by accident — or with default settings. It takes care and attention to detail. And unfortunately, most of what we come across on a daily basis does not constitute good web typography.

In my experience, there are a few challenges to typesetting on the web, outside the much-discussed issues of browser discrepancies and device diversity:

- **Content-creator knowledge.** Many people who are responsible for writing, editing, and entering content for websites simply don’t have a good baseline knowledge of typesetting, particularly for the web.
- **Separation of code and content.** Typesetting involves the interplay of meaning and presentation. In a typical content management system, there is a divide between developers who write the code and authors who write the content. This usually results in a lack of control over the necessary settings.
- **Allure of frameworks.** Design system frameworks, like Bootstrap and Foundation, make admirable efforts to provide general purpose defaults that work in a variety situations. But they still require the knowledge and interplay described above, so it's often easier to settle for what you get out of the box.

On this last point, Brown warns that “being efficient is great, but you should understand the decisions a typographic system makes on your behalf.” What you get by default with most frameworks is never quite satisfying. I understand why, but even with the risks outlined above, I couldn’t help but think there might be a better way to achieve good typography without requiring much knowledge or control.

Using Brown’s words as a guide, I set out to create a simple, lightweight stylesheet that _lays the “foundation for flexible typography that looks good and performs well in many contexts”_ while _being transparent about the decisions being made on your behalf_.

## Considerations

These are a few things I wanted to keep in mind:

- **Respect reader’s font adjustments.** Although Brown doesn't mention accessibility directly in the Readers are Typographers Too section, he does say that typography on the web “has the potential to work for everyone by default.” I intentionally wanted to ensure that things like font sizes are relative to any preferences the reader has set on whatever device they're using.
- **Play nicely with other frameworks.** Since this is not a complete framework, and is intended for use on top of other tools like normalize.css or Bootstrap, my goal was to progressively enhance what you're already using.
- **Allow customization from the markup.** Keeping in mind the separation of concerns you have between code and content in most content management systems, I wanted to allow for easy adjustments of the defaults with a few settings you could access without mucking around in the stylesheet.