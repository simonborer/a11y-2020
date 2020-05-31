---
title: "Week 3 - Join Operations"
date: 2020-06-01T08:47:11+01:00
publishdate: 2020-06-01T08:47:11+01:00
featured_image: venn.png
summary: "This week we'll cover coding INNER JOINs to retrieve rows from multiple tables; the use of a self-join; table aliases; JOIN with implicit INNER JOIN syntax; OUTER JOINs to retrieve rows form multiple tables; the various set operators."
---
<section class="slide-only">
    <h2>Here's what we're going today</h2>
    <ol>
        <li>Your midterm</li>
        <li>OCAS is a go</li>
        <li>Things that have come up</li>
        <li>Theory
            <ol>
                <li>The DOM API</li>
                <li>WAI-ARIA</li>
                <li>Showing and hiding content</li>
                <li>Keyboard control</li>
                <li>Controlling focus</li>
                <li>Personas</li>
                <li>Task analysis</li>
            </ol>
        </li>
        <li>Praxis
            <ol>
                <li>Write your own persona</li>
                <li>Write a commuter task analysis with a partner</li>
            </ol>
        </li>
    </ol>
</section>
<section>
    <h3>Auditing accessibility</h3>
    <p>The W3 provide us with a wonderful list of different accessibility auditing tools, in a wide variety of languages: <a href='https://www.w3.org/WAI/ER/tools/?q=command-line-tool' target='_blank'>https://www.w3.org/WAI/ER/tools/?q=command-line-tool</a>.</p>
    <p>The most commonly used one is the <a href='http://wave.webaim.org/extension/' target='_blank'>WAVE Browser extension</a></p>
    <p>Chrome also has an accessibility audit built in. Go to the devtools > audits > Perform an audit and deselect everything except 'Accessibility'.</p>
    <p>Using either of these tools, run an audit and raise your hand when you find something you don't understand.</p>
</section>
<section class="slide-only">
    <h3>Things that have come up</h3>
    <p><img src='/a11y/assets/images/contrast-ratio.png' alt='Screenshot of the Chrome devtools contrast ratio report in the colour picker'>"</p>
</section>
<section class="slide-only">
    <p><code>*, *:before, *:after {outline: 1px solid red}</code></p>
</section>
<section class="slide-only">
    <h3>Learning CSS layout</h3>
    <p><a href='https://flexboxfroggy.com/'>Flexbox Froggy</a></p>
    <p><a href='https://cssgridgarden.com/'>CSS Grid Garden</a></p>
</section>
<section class="slide-only">
    <h3>The `name` attribute.</h3>
    <p>The <code>name</code> attribute is for use when <code>POST</code>ing or <code>GET</code>ing a form.</p>
    <p>A surprising number of examples of the <code>label</code> element use the same <code>id</code> and <code>name</code> attributes, which is confusing.</p>
    <p>The <code>for</code> attribute of your <code>label</code> element refers to the <code>id</code> of the labelled element.</p>
</section>
<section>
    <h3>The DOM API</h3>
    <p>Both 'DOM' and 'API' are acronyms that get thrown around a lot. Let's quickly make sure we all know what they mean.</p>
    <p>An <strong>Application Programming Interface</strong> is a user interface, where the user is a person writing a computer script. It provides you information and functionality from the document or application that you're interacting with.</p>
    <p>The <strong>Document Object Model</strong> is an API that represents an HTML (or XML) document as a traversable tree structure. The elements (and attributes, including text content) within that structure are referred to as 'nodes'.</p>
</section>
<section>
    <p>There are different kinds of attributes we can assign to DOM nodes. There are native attributes, which are provided by the HTML spec, e.g. <code>class</code>, <code>alt</code>, <code>target</code>. There are data attributes (added in HTML5), which are user-customizable. And there are ARIA attributes.</p>
    <p>ARIA (Accessible Rich Internet Applications) provides contextual information about if and how DOM nodes can update, and what happens when they do.</p>
</section>
<section>
    <h3>When to use ARIA</h3>
    <ol>
        <li class="fragment">There is a DOM node (including text) that can or does update without a page refresh being triggered, and</li>
        <li class="fragment">There is no native semantics or attribute available.</li>
    </ol>
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
    <h3>Accessible tabs are &lt;em&gt;hard&lt;/em&gt;</h3>
    <p>
        <p data-height="265" data-theme-id="0" data-slug-hash="pVBoQx" data-default-tab="js,result" data-user="simonborer" data-embed-version="2" data-pen-title="pVBoQx" class="codepen">See the Pen <a href="https://codepen.io/simonborer/pen/pVBoQx/">pVBoQx</a> by Simon Borer (<a href="https://codepen.io/simonborer">@simonborer</a>) on <a href="https://codepen.io">CodePen</a>.</p>
        <script async src="https://static.codepen.io/assets/embed/ei.js"></script>
    </p>
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
<section>
    <h3>Persona creation process</h3>
    <ol>
        <li class="fragment">Interview and/or observe an adequate number of people.</li>
        <li class="fragment">Find patterns in the interviewees’ responses and actions, and use those to group similar people together.</li>
        <li class="fragment">Create archetypical models of those groups, based on the patterns.</li>
    </ol>
</section>
<section>
    <p><img src='https://media.nngroup.com/media/editor/2018/01/05/personaexample.jpg' alt='Example of a persona document'></p>
</section>
<section>
    <p>Just like any other team tool, personas don't work if you don't have buy-in.</p>
</section>
<section>
    <h3>Aurora Harley</h3>
    <ol>
        <li class="fragment">Name, age, gender, and an image of the persona</li>
        <li class="fragment">A tag line</li>
        <li class="fragment">The experience and relevant skills in the area of the product or service</li>
        <li class="fragment">Some context to indicate how he/she would interact with your product or service (e.g., the voluntariness of use, frequency of use, and preferred device)</li>
        <li class="fragment">Any goals, attitudes, and concerns he/she would have when using your product or service</li>
        <li class="fragment">Quotes or a brief scenario, that indicate the persona’s attitude toward the product or service you’re designing.</li>
    </ol>
</section>
<section>
    <h3>Write your own Persona</h3>
</section>
<section>
    <h3>Task analysis</h3>
    <p>Like many usability techniques, task analysis can happen as a precursor to design, or to test it.</p>
    <p>You should do a rudimentary version of this to break your test scenarios into tasks, but you should also consider doing this when generating results from your tests.</p>
</section>
<section>
    <h3>Task analysis topics</h3>
    <ol>
        <li class="fragment">Trigger: What prompts users to start their task?</li>
        <li class="fragment">Desired Outcome: How users will know when the task is complete?</li>
        <li class="fragment">Base Knowledge: What will the users be expected to know when starting the task?</li>
        <li class="fragment">Required Knowledge: What the users actually need to know in order to complete the task?</li>
        <li class="fragment">Artifacts: What tools or information do the users utilize during the course of the task?</li>
    </ol>
</section>
<section>
    <h3>Task analysis topics</h3>
    <p>With a partner, perform a task analysis of their journey to class today. Use your judgement in determining the level of detail that is appropriate to find efficiences in their journey. Was their journey optimal?</p>
</section>