---
title: "Step 4: The DOM & Assistive Devices"
date: 2020-06-03T08:47:11+01:00
publishdate: 2020-06-03T08:47:11+01:00
featured_image: gadget.jpg
summary: "Today we'll dive into accessibility, looking at the DOM, assistive devices, accessible content, and automated auditing."
---
<section>
    <h2>Here's what we're going to talk about today:</h2>
    <ol>
        <li class="fragment"><a href="#overview">Accessibility overview</a></li>
        <li class="fragment"><a href="#content">Content</a></li>
        <li class="fragment"><a href="#DOM">What is the DOM</a></li>
        <li class="fragment"><a href="#devices">Assistive devices</a></li>
        <li class="fragment"><a href="#auditing">Auditing</a></li>
    </ol>
</section>
<section id="overview">
    <h2>Accessibility overview</h2>
    <p>Accessibility is both a philosophy, and a legal requirement.</p>
    <p><strong>Philosophy</strong>: universal design, removing barriers and creating equity.</p>
    <p><strong>Law</strong>: The Access for Ontarians with Disabilities Act, in accordance with the Canadian Charter of Rights and Freedoms, mandates a level of <abbr title="Web consortium accessibility guidelines">WCAG</abbr> compliance.</p>
</section>
<section>
    <h3>How we follow the WCAG guidelines</h3>
    <p>WCAG compliance mandates semantics, content, proper source order, text alternatives to visual information, accomodations for colour-blindness and low visual acuity, keyboard-only functionality, and the use of the WAI-ARIA specification.</p>
</section>
<section>
    <p><strong>Semantics</strong> in HTML refers to using native elements and attributes for their defined purpose.</p>
    <p>A correct <strong>source order</strong> means that the visual flow of the document matches the source code.</p>
    <p class="codepen" data-height="265" data-theme-id="light" data-default-tab="html,result" data-user="simonborer" data-slug-hash="eYJNEEV" style="height: 265px; box-sizing: border-box; display: flex; align-items: center; justify-content: center; border: 2px solid; margin: 1em 0; padding: 1em;" data-pen-title="eYJNEEV">
    </p>
    <script async src="https://static.codepen.io/assets/embed/ei.js"></script>
    <p style="margin-top:2rem;"><strong>Text alternatives</strong> are provided when information is presented visually - this includes images, graphs, charts and tables, but also cases where elements have implicit functions based on the visual design, i.e. buttons within a form.</p>
    <p class="callout">Refer back to our <a href="https://a11y2020.ca/posts/the-1st-week#componentOfTheWeek" target="_blank">Week 1 "Component of the Week"<span class="show-for-sr"> Opens in a new window</span></a> for a refresher on text alternatives.</p>
</section>
<section>
    <p>We can provide alternatives to this visual information with <code>alt</code> tags for graphic content, <code>scope</code> and <code>caption</code> for tables, and <code>label</code>s or screen reader-specific content for inputs, buttons and links.</p>
    <p>We must also keep in mind that our elements are often used as navigational landmarks for people using non-visual clients, including headers for document structure.</p>
</section>
<section>
    <p>Because not all visual impairments require the use of a screenreader, we provide <strong>alternatives to colour cues</strong> for people with colour-blindness (i.e. focus outline, proper labelling), and for people with reduced visual abilities we check our <strong>colour contrast ratios</strong> and test our websites for up to <strong>200% zoom</strong>.</p>
    <figure>
        <img src="/images/color-checker.png" alt="">
        <figcaption>Not sure if you color contrast is up to snuff? The quickest way to check is by clicking on the text's "colour sample" in your browser tools.</figcaption>
    </figure>
</section>
<section>
    <p>For people with motor-impairment issues, we ensure that we do not disable the native functionality of our proper semantic HTML, and where native functionality is not available, we create <strong>keyboard events</strong> to supplement our click events.</p>
    <p>We also maintain our tab order by having our source order properly represented.</p>
    <p>On those rare occasions where our visual order and source order are in conflict, we can control focus with Javascript.</p>
    <p class="codepen" data-height="265" data-theme-id="light" data-default-tab="html,result" data-user="simonborer" data-slug-hash="gOPpxmb" style="height: 265px; box-sizing: border-box; display: flex; align-items: center; justify-content: center; border: 2px solid; margin: 1em 0; padding: 1em;" data-pen-title="gOPpxmb"></p>
    <script async src="https://static.codepen.io/assets/embed/ei.js"></script>
    <p>Where we want to make an element focusable that does not have native focusability, we can use the <code>tabindex='0'</code> attribute value.</p>
</section>
<section>
    <p>The <strong><abbr title="Web Accessibility Initiative ">WAI-ARIA</abbr></strong> specification allows us to supplement our HTML elements, widgets and document presentation by defining roles and properties for screenreader users.</p>
    <p>This is especially important when updating content on the page without a location change or page refresh, which is a common practice when using modern front-end javascript frameworks, such as Angular, React, and Vue.</p>
</section>
<section>
    <p>Of course we keep in mind that all these standards apply whether on a desktop or mobile device, with a few special considerations for mobile, including...</p>
    <ol>
        <li class="fragment">Maintaining keyboard functionality</li>
        <li class="fragment">Supporting different orientations</li>
        <li class="fragment">Touch target size and spacing</li>
        <li class="fragment">Gesture alternatives, and </li>
        <li class="fragment">Appropriate virtual keyboard data types.</li>
    </ol>
</section>
<section>
    <p>In order to enforce accessibility compliance and best practices, we need to help our team mates understand these techniques. We can encourage our team to use <strong>manual testing tools</strong> like the <a href="https://www.deque.com/axe/" target="_blank">aXe browser plugin<span class="show-for-sr"> Opens in a new window</span></a>, incorporate <strong>linting</strong> into our build process and <strong>auditing</strong> into our deployment or site monitoring</p>
    <p>Additionally, because some accessibility techniques, especially ARIA, are context-dependent, automated enforcement can be a challenge. Manual <strong>code review</strong> is an essential part of making our whole team stronger and our product better.</p>
</section>
<section>
    <h3>Don&#39;t be redundant</h3>
    <p><code>div[role='button']</code> is not redundant, but <code>button[role='button']</code> <em>is</em> redundant.</p>
</section>
<section>
    <h3>Want to be safe?</h3>
    <p>TEST</p>
    <p>I can't emphasize enough how important it is to test. That's why there are QA departments. It is wonderful to follow best practices, but even when specification documentation is perfect (it's not), and even when you limit your scope to the latest versions of a few popular clients (don't), and even when your linters catch all the edge cases (they won't), you still makes mistakes.</p>
</section>
<section>
    <h3>Tabindex</h3>
    <p><code>tabindex</code> is an attribute that specifies <em>focusability</em>. Focus is usually stepped through with the <code>tab</code> key, hence the name.</p>
    <p><code>tabindex="-1"</code> is focusable, but not sequentially. As in, you can`t tab to it.</p>
    <p><code>tabindex="0"</code> means that the element is focusable in the normal tab sequence.</p>
    <p><code>tabindex="1"</code>, or any other positive value, means that this element takes precedence over any other element without a declared tabindex. If you are using this, that`s a bad sign.</p>
</section>
<section>
    <p>Remember not to confuse the visual order with the DOM order :)</p>
    <p>Declaring a tabindex value can affect scrolling behaviour on child elements. For examples, see <a href="https://jsfiddle.net/jainakshay/0b2q4Lgv/">https://jsfiddle.net/jainakshay/0b2q4Lgv/</a></p>
</section>
<section id="content">
    <h2>Making content accessible</h2>
    <p>Accessible <strong>content</strong> means...</p>
    <ol>
        <li class="fragment">Unique page titles (as it can be difficult to assess if the page has actually changed otherwise)</li>
        <li class="fragment">Concise link text (as screen readers read them in their entirety)</li>
        <li class="fragment">Text-based information about link behaviour</li>
        <li class="fragment">Skippable navigation</li>
        <li class="fragment">Captions and transcriptions that contain all relevant visual information</li>
        <li class="fragment">Verbose error messages (that capture focus), and</li>
        <li class="fragment">Using words rather than ASCII symbols</li>
    </ol>
</section>
<section>
    <h3>Accessible content - page titles</h3>
    <p>Page title should be unique and descriptive. If it's page 2 of 3, say so.</p>
</section>
<section>
    <h3>Accessible content - headings</h3>
    <p>Headings should structure your document. Think of the way your information is structured - it's very rarely appropriate to have just an h1 and then p tags all the way down. Headings should provide meaning and context.</p>
</section>
<section>
    <h3>Accessible content - alt text</h3>
    <p>Alternative text should be your best effort to convey <em>all</em> of the relevant information in the image - no more, no less. This gets tricky when you get into things like graphs. Think of how WebAIM approached it in our reading this week.</p>
</section>
<section>
    <h3>Accessible content - transcripts and captions</h3>
    <p>Audio and video need transcriptions and/or captions. Keep an ear out for sounds that convey relevant information, and make sure they're included - not just the words.</p>
</section>
<section>
    <h3>Accessible content - beware things that look like text</h3>
    <p>Be on the lookout for images with embedded text, or worse - OCR-resistant PDFs.</p>
</section>
<section>
    <h3>Accessible content - ASCII</h3>
    <p>Think about what this sounds like: ¯\_(ツ)_/¯.</p>
    <p>For the same reason, write "16 to 17 years old" instead of "16-17 years old".</p>
</section>
<section>
    <h3>Accessible content - links</h3>
    <p>Via <a href='https://www.sitepoint.com/15-rules-making-accessible-links/' target='_blank'>sitepoint</a></p>
    <ol>
        <li class="fragment">Don&#39;t say they&#39;re links - the screenreader tells you</li>
        <li class="fragment">Don&#39;t capitalize - screenreaders will read them out letter by letter</li>
        <li class="fragment">Don&#39;t make the link text the url</li>
        <li class="fragment">Keep links short - screenreaders won&#39;t skip them.</li>
        <li class="fragment">Identify link behaviour - i.e. downloads, new windows, anchor links</li>
        <li class="fragment">Don&#39;t embed link types identifications in your CSS</li>
        <li class="fragment">Don&#39;t abuse javascript to do link-ish things with elements that aren&#39;t links (anchors or area tags)</li>
        <li class="fragment">If an image is inside an anchor tag, it&#39;s alt text should refer to the link behaviour, as well as the image&#39;s information.</li>
        <li class="fragment">Empty or broken links are just mean.</li>
    </ol>
</section>
<section id="DOM">
    <h2>The DOM API</h2>
    <p>Both 'DOM' and 'API' are acronyms that get thrown around a lot. Let's quickly make sure we all know what they mean.</p>
    <p>An <strong>Application Programming Interface</strong> is a user interface, where the user is a person writing a computer script. It provides you information and functionality from the document or application that you're interacting with.</p>
    <p>The <strong>Document Object Model</strong> is an API that represents an HTML (or XML) document as a traversable tree structure. The elements (and attributes, including text content) within that structure are referred to as 'nodes'.</p>
</section>
<section>
    <p>There are different kinds of attributes we can assign to DOM nodes. There are native attributes, which are provided by the HTML spec, e.g. <code>class</code>, <code>alt</code>, <code>target</code>. There are data attributes (added in HTML5), which are user-customizable. And there are ARIA attributes.</p>
    <p>ARIA (Accessible Rich Internet Applications) provides contextual information about if and how DOM nodes can update, and what happens when they do.</p>
</section>
<section id="">
    <h3>When to use ARIA</h3>
    <ol>
        <li class="fragment">There is a DOM node (including text) that can or does update without a page refresh being triggered, and</li>
        <li class="fragment">There is no native semantics or attribute available.</li>
    </ol>
</section>
<section>
    <h3>What ARIA attributes?</h3>
    <p>You can find a pretty comprehensive list at <a href='https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/ARIA_Techniques'>https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/ARIA_Techniques</a></p>
    <p>There are a lot, but you should know about the <code>role</code> attribute, which labels interactive elements, including tabs, search, form, and grid; and state attributes including <code>aria-live</code>, <code>aria-expanded</code>, and <code>aria-hidden</code> (which differs from the native <code>hidden</code> attribute).</p>
</section>
<section>
    <h3>Showing &amp; hiding</h3>
    <p>
        <p data-height="463" data-theme-id="0" data-slug-hash="xjBoWv" data-default-tab="result" data-user="simonborer" data-embed-version="2" data-pen-title="Hiding Techniques" class="codepen">See the Pen <a href="https://codepen.io/simonborer/pen/xjBoWv/">Hiding Techniques</a> by Simon Borer (<a href="https://codepen.io/simonborer">@simonborer</a>) on <a href="https://codepen.io">CodePen</a>.</p>
        <script async src="https://static.codepen.io/assets/embed/ei.js"></script>
    </p>
</section>
<section>
    <h3>WAI-ARIA deep dive</h3>
    <p>As we covered earlier, WAI-ARIA, a.k.a. ARIA, is a specification from the W3C that uses element attributes to supplement existing semantics <ol>
            <li>to provide more information about your markup, and</li>
            <li>provide information about content that updates without a page refresh.</li>
    </p>
    <p>This is especially relevant when you are using a front-end javascript framework (Angular, React, Vue, et al.).</p>
</section>
<section>
    <p>Remember that the spec tells us that we should use native semantics when they are available.</p>
    <p>If it's a button, use a < button>.</p>
</section>
<section>
    <h3>ARIA roles</h3>
    <p>The role attribute provides information about an element's purpose.</p>
    <p>The role attribute identifies the element to the screenreader, but it <em>does not</em> recreate the native functionality. That's on you.</p>
</section>
<section>
    <h3>role=&#34;button&#34;</h3>
    <p>Let's say, for whatever reason, you need to make a button out of something that's not < button>,
            < input type='button' />,
            < input type='submit' />,
            < input type='reset' /> or
            < input type='image' />.</p>
    <p><code>role='button'</code> identifies any element as a button to a screenreader. Use this in conjunction with <code>tabindex='0'</code> - the role itself does not make the element focusable.</p>
    <p>Remember, too, that a native HTML button will fire an onclick event when space or enter are pressed - so you're also responsible for recreating that native functionality.</p>
</section>
<section>
    <h3>More roles! - widgets</h3>
    <p><code>checkbox</code></p>
    <p><code>dialog</code> (this can be a modal, or not)</p>
    <p><code>link</code></p>
    <p><code>log</code> (i.e. a chat log)</p>
    <p><code>marquee</code> (like a <code>log</code>, but not vital or linear, i.e. a carousel or stock ticker)</p>
    <p><code>progressbar</code></p>
    <p><code>radio</code></p>
    <p><code>scrollbar</code></p>
</section>
<section>
    <p><code>slider</code> (i.e. a range slider or volume control)</p>
    <p><code>spinbutton</code> (a value selection input with up and down arrows)</p>
    <p><code>status</code> (a status update message, i.e. `your changes have been saved`</p>
    <p><code>tablist</code> > <code>tab</code> + <code>tabpanel</code></p>
    <p><code>grid</code> > <code>row</code> > <code>rowheader</code> + <code>cell</code> + <code>columnheader</code></p>
    <p><code>menubar</code> > <code>menu</code> > <code>menuitem</code> + <code>menuitemcheckbox</code></p>
    <p><code>textbox</code></p>
    <p><code>timer</code></p>
    <p><code>tooltip</code></p>
</section>
<section>
    <p><code>tree</code>/<code>treegrid</code> > <code>treeitem</code></p>
    <p><code>switch</code> identical to <code>checkbox</code>, but strictly for values of on or off</p>
    <p><code>listbox</code> > <code>option</code></p>
    <p><code>radiogroup</code> > <code>radio</code></p>
</section>
<section>
    <h3>Even more roles! - document structure</h3>
    <p><code>article</code></p>
    <p><code>definition</code></p>
    <p><code>directory</code> (i.e. table of contents)</p>
    <p><code>document</code></p>
    <p><code>group</code> (of UI elements not in a perceivable page section)</p>
    <p><code>heading</code></p>
    <p><code>img</code> (useful in case of background images)</p>
    <p><code>list</code> > <code>listitem</code></p>
</section>
<section>
    <p><code>math</code> (there is an entire markup language for mathy stuff! it's called <a href='https://www.w3.org/Math/whatIsMathML.html' target='_blank'>MathML</a> and can be called into other markup, like HTML)</p>
    <p><code>note</code></p>
    <p><code>presentation</code> - similar in function to aria-hidden; this tells the screenreader that the element is decorative, but <a href='http://john.foliot.ca/aria-hidden/' target='_blank'>support for it on natively focusable elements is interesting</a>.</p>
    <p><code>region</code></p>
    <p><code>separator</code></p>
    <p><code>toolbar</code></p>
</section>
<section>
    <h3>And finally... more roles! - landmarks</h3>
    <p><code>application</code> - for when your HTML document behaves completely different from a standard html document; probably don't use this. It turns off all standard keyboard shortcuts in most screenreaders.</p>
    <p><code>banner</code> - analogous to < header>
    </p>
    <p><code>complementary</code> - like < aside>
    </p>
    <p><code>contentinfo</code> - like < footer>
    </p>
    <p><code>form</code></p>
    <p><code>main</code></p>
    <p><code>navigation</code></p>
    <p><code>search</code></p>
</section>
<section>
    <h3>Widget attributes</h3>
    <p><code>role="combobox|textbox" aria-autocomplete="none|inline|list|both"</code></p>
    <p><code>role="checkbox|switch|..." aria-checked="true|false|mixed"</code></p>
    <p><code>aria-current="page|step|date|location|time|true|false"</code></p>
    <p><code>aria-disabled="true|false"</code></p>
    <p>aria-expanded="true|false"</code></p>
    <p><code>aria-haspopup="true|false|menu|listbox|tree|grid|dialog"</code></p>
    <p><code>aria-hidden="true|false|undefined"</code></p>
    <p><code>aria-invalid="true|false|grammar|spelling"</code></p>
    <p><code>aria-label={string}</code> only for invisible text</p>
</section>
<section>
    <p><code>role="grid|heading|listitem|row|tablist" aria-level={integer}</code></p>
    <p><code>role="textbox" aria-multiline="true|false"</code></p>
    <p><code>role="grid|listbox|tablist|tree" aria-multiselectable="true|false"</code></p>
    <p><code>role="scrollbar|select|separator|slider|tablist|toolbar" aria-orientation="horizontal|vertical|undefined"</code></p>
    <p><code>role="button" aria-pressed="true|false|mixed"</code></p>
    <p><code>role=checkbox|combobox|grid|gridcell|listbox|radiogroup|slider|spinbutton|textbox" aria-readonly="true|false"</code></p>
    <p><code>role="combobox|gridcell|listbox|radiogroup|spinbutton|textbox|tree" aria-required="true|false"</code></p>
    <p><code>role="gridcell|option|row|tab" aria-selected="true|false|undefined"</code></p>
</section>
<section>
    <p><code>role="columnheader|rowheader" aria-sort="ascending|descending|none|other"</code></p>
    <p><code>role="range|scrollbar|separator|slider|spinbutton" aria-valuemax={number} aria-valuemin={number} aria-valuenow={number}</code></p>
    <p><code>role="range|separator" aria-valuetext={string}</code></p>
</section>
<section>
    <h3>Live region attributes</h3>
    <p><code>aria-live="polite|assertive|off"</code></p>
    <p><code>aria-live="polite" aria-atomic="true|false"</code></p>
    <p><code>aria-live="polite" aria-relevant="additions|text|removals|all"</code></p>
    <p><code>aria-live="assertive" aria-busy="true|false"</code></p>
</section>
<section>
    <h3>Implicit live region attributes</h3>
    <p>Several roles have implicit live region values:</p>
    <p><code>role="alert"</code> has an implicit <code>aria-live="assertive"</code></p>
    <p><code>role="status"</code> and <code>role="log"</code> have an implicit <code>aria-live="polite"</code></p>
    <p><code>role="timer"</code> and <code>role="marquee"</code> have an implicit <code>aria-live="off"</code></p>
    <p>These can be overridden by explicitly declaring <code>aria-live</code> values.</p>
</section>
<section>
    <h3>Relationship attributes</h3>
    <p><code>role="application|composite|group|textbox" aria-activedescendant={id}</code></p>
    <p><code>aria-controls={id}</code></p>
    <p><code>aria-describedby={id}</code> similar to <code>aria-labelledby</code>, but verbose instead of concise</p>
    <p><code>aria-labelledby={id}</code></p>
    <p><code>aria-flowto={id}</code> gives the user the option to move to an element, overriding the source order</p>
</section>
<section>
    <p><code>aria-owns={id}</code> Defines a parent-child relationship when one isn't semantically apparent. To understand how this is different from <code>aria-controls</code>, imagine a carousel. The arrows on the left and right would have <code>aria-controls</code> attributes. The dots at the bottom that correlate to individual slides would have <code>aria-owns</code> attributes.</p>
    <p><code>role="article|listitem|menuitem|option|radio|tab" aria-setsize={integer} aria-posinset={integer}</code> Only required when not all elements from the set are included in the DOM.</p>
</section>