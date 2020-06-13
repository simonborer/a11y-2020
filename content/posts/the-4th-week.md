---
title: "Step 4: The DOM & Assistive Devices"
date: 2020-06-03T08:47:11+01:00
publishdate: 2020-06-03T08:47:11+01:00
featured_image: gadget.jpg
summary: "Today we'll dive into accessibility, looking at the DOM, assistive devices, accessible content, and automated auditing."
---
<section>
    <h2>Here's what we're going to talk about today:</h2>
    <ol role="directory">
        <li class="fragment"><a href="#overview">Accessibility overview</a></li>
        <li class="fragment"><a href="#devices">Assistive devices</a></li>
        <li class="fragment"><a href="#DOM">What is the DOM</a></li>
        <li class="fragment"><a href="#content">Content</a></li>
        <li class="fragment"><a href="#auditing">Accessibility workflow</a></li>
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
    <p>WCAG compliance mandates: 
        <ul><li>semantics,</li> <li>proper source order,</li> <li>content considerations,</li> <li>text alternatives to visual information,</li> <li>accomodations for colour-blindness and low visual acuity,</li> <li>keyboard-only functionality, and </li><li>the use of the WAI-ARIA specification.</li></ul></p>
</section>
<section id="devices">
    <h2>Assistive Devices</h2>
    <figure>
        <img src="/images/massage.jpg" alt="electric circuitry, an extension of the central nervous system. Media, by altering the nvironment, evoke in us unique ratios of sense perceptions. The extension of any one sense alters the way we think and act - the way we perceive the world. When these ratios change, men change.">
        <figcaption>Aside from the dated language (people change, not just men), Marshall McLuhan is <em>definitely someone you should be familiar with</em>, as technologists, and as people who like Canada.</figcaption>
    </figure>
</section>
<section>
    <figure style="display: flex;flex-wrap: wrap;justify-content: center;"><img style="object-fit: cover;max-width: 50%;" src="/images/mouse.jpg" alt="Computer mouse"><img style="object-fit: cover;max-width: 50%;" src="/images/keyboard.jpg" alt="Computer keyboard"><figcaption class="post-only">Two popular assistive devices</figcaption></figure>
    <p>People are accessing your web content with assistive devices. The beauty of writing your code to standards is <strong>you don't need to know <em>which</em> devices</strong>.</p>
</section>
<section>
    <p>It could be this one...</p>
    <video style="max-width: 100%;" id="vid" controls data-iterations="1" autoplay="true"><source src="/video/eyegaze.mp4" type="video/mp4" />Your browser does not support the video tag.</video>
    <script type="text/javascript">
        var vid = document.getElementById('vid');
        var i = vid.dataset.iterations;
        vid.addEventListener('ended', function () {    
            if (i < 5) {       
                this.currentTime = 0;
                this.play();
                i ++;
                vid.dataset.iterations = i;
            }   
        }, false);
    </script>
</section>
<section>
    <p style="margin-top:1rem">...or this one <br><img src="/images/air.gif" alt="Sip-and-puff system"></p>
</section>
<section>
    <p>...or this one <br><img src="/images/braille-keyboard.jpg" alt="Braille keyboard"></p>
</section>
<section>
    <p>...or this one <br><img src="/images/red-button.png" alt="Big red button"></p>
</section>
<section>
    <p>...or this one <br><a href="https://www.core77.com/posts/20361/shikun-suns-drawbraille-phone-concept-for-the-blind-20361" target="_blank"><img src="/images/braille-phone.jpg" alt="Braille phone"><span class="show-for-sr"> Opens in a new window</span></a></p>
</section>
<section>
    <p>And that's just <em>hardware</em>. When it comes to software, we see principles like <a href="https://css-tricks.com/the-difference-between-responsive-and-adaptive-design/" target="_blank">responsive design<span class="show-for-sr"> Opens in a new window</span></a> and <a href="https://alistapart.com/article/understandingprogressiveenhancement/" target="_blank">progressive enhancement<span class="show-for-sr"> Opens in a new window</span></a>, which both start with the idea that <em>you don't know how your content will be viewed</em>. </p>
    <p><figure>
        <img src="/images/w3m.png" alt="This web page in a text-based browser.">
        <figcaption>Sometimes it's like this, for example.</figcaption>
    </figure></p>
</section>
<section>
    <p>At the risk of sounding like my aunts on facebook - you can't control how others see you (or your code). You just have to do what is right (according to the <a href="https://www.w3.org/standards/" target="_blank">W3C Web Standards<span class="show-for-sr"> Opens in a new window</span></a>).</p>
</section>
<section id="DOM">
    <h2>The DOM API</h2>
    <p>How is it that our code can rise to meet all these wonderful devices? Via the DOM API!</p>
    <p>Both 'DOM' and 'API' are acronyms that get thrown around a lot. Let's quickly make sure we all know what they mean.</p>
    <p>An <strong>Application Programming Interface</strong> is a user interface, where the user is a person writing a computer script. It provides you information and functionality from the document or application that you're interacting with.</p>
    <p>The <strong>Document Object Model</strong> is an API that represents an HTML (or XML) document as a traversable tree structure. The elements (and attributes, including text content) within that structure are referred to as 'nodes'.</p>
</section>
<section>
    <p>There are different kinds of attributes we can assign to DOM nodes. There are native attributes, which are provided by the HTML spec, e.g. <code>class</code>, <code>alt</code>, <code>target</code>. There are data attributes (added in HTML5), which are user-customizable. And there are ARIA attributes.</p>
    <p>ARIA (Accessible Rich Internet Applications) provides contextual information about if and how DOM nodes can update, and what happens when they do.</p>
</section>
<section>
    <h3>WAI-ARIA</h3>
    <p>The <strong><abbr title="Web Accessibility Initiative ">WAI-ARIA</abbr></strong> specification allows us to supplement our HTML elements, widgets and document presentation by defining roles and properties for screenreader users.</p>
    <p>This is especially important when updating content on the page without a location change or page refresh, which is a common practice when using modern front-end javascript frameworks, such as Angular, React, and Vue.</p>
</section>
<section id="">
    <h3>When to use ARIA</h3>
    <ol>
        <li class="fragment">There is visual information on the page that has no native text alternative format, or</li>
        <li class="fragment">There is a DOM node (including text) that can or does update without a page refresh being triggered, and</li>
        <li class="fragment">There is no native semantics or attribute available.</li>
    </ol>
</section>
<section>
    <h3>What ARIA attributes should I use?</h3>
    <p>You can find a pretty comprehensive list on <a href="https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/ARIA_Techniques" target="_blank">MDN<span class="show-for-sr"> Opens in a new window</span></a></p>
    <p>There are a lot, but you should know about the <code>role</code> attribute, which labels interactive elements, including tabs, search, form, and grid; and state attributes including <code>aria-live</code>, <code>aria-expanded</code>, and <code>aria-hidden</code> (which differs from the native <code>hidden</code> attribute).</p>
</section>
<section id="content">
    <h2>Making content accessible</h2>
    <p>We can provide alternatives to this visual information with <code>alt</code> tags for graphic content, <code>scope</code> and <code>caption</code> for tables, and <code>label</code>s or screen reader-specific content for inputs, buttons and links.</p>
    <p>We must also keep in mind that our elements are often used as navigational landmarks for people using non-visual clients, including headers for document structure.</p>
</section>
<section>
    <p style="margin-top:2rem;"><strong>Text alternatives</strong> are provided when information is presented visually - this includes images, graphs, charts and tables, but also cases where elements have implicit functions based on the visual design, i.e. buttons within a form.</p>
    <p class="callout">Refer back to our <a href="https://a11y2020.ca/posts/the-1st-week#componentOfTheWeek" target="_blank">Week 1 "Component of the Week"<span class="show-for-sr"> Opens in a new window</span></a> for a refresher on text alternatives.</p>
</section>
<section>
    <p>Accessible <strong>text content</strong> means...</p>
    <ol>
        <li class="fragment">Unique page titles (as it can be difficult to assess if the page has actually changed otherwise)</li>
        <li class="fragment">Concise link text (as screen readers read them in their entirety)</li>
        <li class="fragment">Text-based information about link behaviour</li>
        <li class="fragment">Skippable navigation</li>
        <li class="fragment">Captions, transcriptions and other alternative text that contain all relevant visual information</li>
        <li class="fragment">Verbose error messages (that capture focus), and</li>
        <li class="fragment">Using words rather than ASCII symbols</li>
    </ol>
</section>
<section>
    <h3>Page titles</h3>
    <p>Page title should be unique and descriptive. If it's page 2 of 3, say so.</p>
</section>
<section>
    <h3>Headings</h3>
    <p>Headings should structure your document. Think of the way your information is structured - it's very rarely appropriate to have just an h1 and then p tags all the way down. Headings should provide meaning and context.</p>
</section>
<section>
    <h3>Alt text</h3>
    <p>Alternative text should be your best effort to convey <em>all</em> of the relevant information in the image - no more, no less. This gets tricky when you get into things like graphs. Think of how WebAIM approached it in our reading this week.</p>
</section>
<section>
    <h3>Transcripts and captions</h3>
    <p>Audio and video need transcriptions and/or captions. Keep an ear out for sounds that convey relevant information, and make sure they're included - not just the words.</p>
</section>
<section>
    <h3>Beware things that look like text</h3>
    <p>Be on the lookout for images with embedded text, or worse - OCR-resistant PDFs.</p>
</section>
<section>
    <h3>ASCII</h3>
    <p>Think about what this sounds like: ¯\_(ツ)_/¯.</p>
    <p>For the same reason, write "16 to 17 years old" instead of "16-17 years old".</p>
</section>
<section>
    <h3>Links</h3>
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
<section>
    <p>Because not all visual impairments require the use of a screenreader, we provide <strong>alternatives to colour cues</strong> for people with colour-blindness (i.e. focus outline, proper labelling), and for people with reduced visual abilities we check our <strong>colour contrast ratios</strong> and test our websites for up to <strong>200% zoom</strong>.</p>
</section>
<section>
    <figure>
        <img src="/images/color-checker.png" alt="" style="border:2px solid rgba(255,255,255,.75)">
        <figcaption>Not sure if you color contrast is up to snuff? The quickest way to check is by clicking on the text's "colour sample" in your browser tools.</figcaption>
    </figure>
</section>
<section>
    <h3>Semantic HTML</h3>
    <p>Accessible <strong>documents</strong> are traversable</p>
    <p><strong>Semantics</strong> in HTML refers to using native elements and attributes for their defined purpose.</p>
    <p>A correct <strong>source order</strong> means that the visual flow of the document matches the source code.</p>
    <p class="codepen" data-height="265" data-theme-id="light" data-default-tab="html,result" data-user="simonborer" data-slug-hash="eYJNEEV" style="height: 265px; box-sizing: border-box; display: flex; align-items: center; justify-content: center; border: 2px solid; margin: 1em 0; padding: 1em;" data-pen-title="eYJNEEV">
    </p>
    <script async src="https://static.codepen.io/assets/embed/ei.js"></script>
</section>
<section>
    <h3>Showing &amp; hiding</h3>
    <p>
        <p data-height="463" data-theme-id="0" data-slug-hash="xjBoWv" data-default-tab="result" data-user="simonborer" data-embed-version="2" data-pen-title="Hiding Techniques" class="codepen">See the Pen <a href="https://codepen.io/simonborer/pen/xjBoWv/">Hiding Techniques</a> by Simon Borer (<a href="https://codepen.io/simonborer">@simonborer</a>) on <a href="https://codepen.io">CodePen</a>.</p>
        <script async src="https://static.codepen.io/assets/embed/ei.js"></script>
    </p>
</section>
<section>
    <p><code>tabindex</code> is an attribute that specifies <em>focusability</em>. Focus is usually stepped through with the <code>tab</code> key, hence the name.</p>
    <p><code>tabindex="-1"</code> is focusable, but not sequentially. As in, you can`t tab to it.</p>
    <p><code>tabindex="0"</code> means that the element is focusable in the normal tab sequence.</p>
    <p><code>tabindex="1"</code>, or any other positive value, means that this element takes precedence over any other element without a declared tabindex. If you are using this, that`s a bad sign.</p>
</section>
<section>
    <p>Remember not to confuse the visual order with the DOM order :)</p>
    <p>Declaring a tabindex value can affect <a href="https://jsfiddle.net/jainakshay/0b2q4Lgv/" target="_blank">scrolling behaviour on child elements<span class="show-for-sr"> Opens in a new window</span></a>.</p>
</section>
<section>
    <p>For people with motor-impairment issues, we ensure that we do not disable the native functionality of our proper semantic HTML, and where native functionality is not available, we create <strong>keyboard events</strong> to supplement our click events.</p>
    <p>We also maintain our tab order by having our source order properly represented.</p>
</section>
<section>
    <p>On those rare occasions where our visual order and source order are in conflict, we can control focus with Javascript.</p>
    <p class="codepen" data-height="265" data-theme-id="light" data-default-tab="html,result" data-user="simonborer" data-slug-hash="gOPpxmb" style="height: 265px; box-sizing: border-box; display: flex; align-items: center; justify-content: center; border: 2px solid; margin: 1em 0; padding: 1em;" data-pen-title="gOPpxmb"></p>
    <script async src="https://static.codepen.io/assets/embed/ei.js"></script>
    <p style="margin-top:2rem;">Where we want to make an element focusable that does not have native focusability, we can use the <code>tabindex='0'</code> attribute value.</p>
</section>
<section>
    <h3>Mobile/touchscreens</h3>
    <p>Of course we keep in mind that all these standards apply whether on a desktop or mobile device, with a few special considerations for mobile, including...</p>
    <ol>
        <li class="fragment">Maintaining keyboard functionality</li>
        <li class="fragment">Supporting different orientations</li>
        <li class="fragment">Touch target size and spacing</li>
        <li class="fragment">Gesture alternatives, and </li>
        <li class="fragment">Appropriate virtual keyboard data types.</li>
    </ol>
</section>
<section id="auditing">
    <h2>Accessibility workflow</h2>
    <p>In order to enforce accessibility compliance and best practices, we need to help our team mates understand these techniques. We can encourage our team to use <strong>manual testing tools</strong> like the <a href="https://www.deque.com/axe/" target="_blank">aXe browser plugin<span class="show-for-sr"> Opens in a new window</span></a>, incorporate <strong>linting</strong> into our build process and <strong>auditing</strong> into our deployment or site monitoring</p>
    <p>Additionally, because some accessibility techniques, especially ARIA, are context-dependent, automated enforcement can be a challenge. Manual <strong>code review</strong> is an essential part of making our whole team stronger and our product better.</p>
</section>
<section>
    <strong>Want to be safe?</strong>
    <p><mark><strong><em style="line-height:2;font-size:1.5rem;">TEST&nbsp;</em></strong></mark></p>
    <p>I can't emphasize enough how important it is to test. That's why there are QA departments. It is wonderful to follow best practices, but even when specification documentation is perfect (it's not), and even when you limit your scope to the latest versions of a few popular clients (don't), and even when your linters catch all the edge cases (they won't), you still makes mistakes.</p>
</section>
<section id="auditing">
    <h2>Auditing</h2>
    <p>Over the next couple weeks we'll learn why <strong>accessibility auditing can never be fully automated</strong>, but today, we're going to look at two handy, light-weight tools for quickly checking to see if there are any obvious accessibility errors on a page.</p>
</section>
<section>
    <p>Open Chrome, and open the developer tools.</p>
    <figure><img src="/images/lighthouse-tab.png" alt=""><figcaption>Across the top, you'll find an option called 'Lighthouse' (or 'Audits' in older versions of Chrome).</figcaption></figure>
</section>
<section>
    <figure>
        <img src="/images/lighthouse-options.png" alt="">
        <figcaption>For our purposes today, you can deselect all the audits aside from 'accessibility', and run the test on 'desktop'.</figcaption>
    </figure>
</section>
<section>
    <figure>
        <img src="/images/lighthouse-results.png" alt="">
        <figcaption>Click 'generate' and get the results!</figcaption>
    </figure>
</section>
<section>
    <figure>
        <img src="/images/lighthouse-negative-results.png" alt="">
        <figcaption>Of course, if you <em>don't</em> get a score of 100%, you can see where "points" were deducted, and learn more about how to fix those violations.</figcaption>
    </figure>
</section>
<section>
    <p>Lighthouse <a href="https://medium.com/pulsar/which-accessibility-testing-tool-should-you-use-e5990e6ef0a" target="_blank">isn't the best<span class="show-for-sr"> Opens in a new window</span></a> tool out there, though. <a href="https://www.deque.com/" target="_blank">Deque<span class="show-for-sr"> Opens in a new window</span></a> is widely considered the industry leader in accessibility consulting. They built the <a href="https://github.com/dequelabs/axe-core" target="_blank">open-source ruleset<span class="show-for-sr"> Opens in a new window</span></a> that the Lighthouse accessibility audit is based on, and their own <a href="https://www.deque.com/axe/" target="_blank">browser extension<span class="show-for-sr"> Opens in a new window</span></a> is considered the best tool for automated auditing of single pages.</p>
</section>
<section>
    <h3>Let's try it out!</h3>
    <ol>
        <li>Download this <a href="/supplemental/fix-my-a11y.html" target="_blank" download>HTML document<span class="show-for-sr"> Downloads a web page, or opens in a new window</span></a>.</li>
        <li>If you haven't already, <a href="https://nodejs.org/en/download/" target="_blank">install Node.js<span class="show-for-sr"> Opens in a new window</span></a></li>
        <li>If you haven't already, open terminal or cmd and run <code>npm install http-server -g</code></li>
        <li>In the terminal, run <code>http-server <em>[the path to the directory containing fix-my-a11y.html]</em> -p 1337</code></li>
        <li>Now you should be able to access your files (via something like http://localhost:1337/fix-my-a11y.html) in Chrome, and run Lighthouse and the aXe browser extension to diagnose errors.</li>
        <li>Open the downloaded html document in a code editor, and alter the HTML until you've resolved all the errors.</li>
    </ol>
</section>